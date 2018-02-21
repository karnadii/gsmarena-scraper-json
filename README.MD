# GSMArena Crawler
crawl gsmarena then return a json object

```bash
npm install
node index.js
```


## Brands
Get list of all brands

Endpoint ```/gsmarena/brands```


```json
[
    {
        "name":"Acer",
        "devices":"99",
        "url":"acer-phones-59.php"
    }
]
```

## Brand detail
get list of phones from certain brand.
Endpoints ``/gsmarena/brand/:url``
example ``/gsmarena/brand/acer-phones-59.php``
```json
{
  "data": [
    {
      "name": "Iconia Talk S",
      "img": "https://cdn2.gsmarena.com/vv/bigpic/acer-iconia-talk-s.jpg",
      "url": "acer_iconia_talk_s-8306.php",
      "description": "Acer Iconia Talk S Android tablet. Announced Aug 2016. Features 7.0″ IPS LCD display, MT8735 chipset, 13 MP primary camera, 2 MP front camera, 3400 mAh battery, 32 GB storage, 2 GB RAM."
    }
  ],
  "next": "acer-phones-f-59-0-p2.php",
  "prev": "#1"
}
```

## Phone detail
get phone spec detail
endpoint ``/gsmarena/phone/:phone``, example ``/gsmarena/phone/acer_iconia_talk_s-8306.php``

```json
{
  "title": "Acer Iconia Talk S",
  "img": "https://cdn2.gsmarena.com/vv/bigpic/acer-iconia-talk-s.jpg",
  "img_url": "acer_iconia_talk_s-pictures-8306.php",
  "spec_detail": [
    {
      "category": "Network",
      "specs": [
        {
          "name": "Technology",
          "value": "GSM / HSPA / LTE"
        }
      ]
    }
  ],
  "quick_spec": {
    "display_size": "7.0\"",
    "display_res": "720x1280 pixels",
    "camera_pixels": "13MP\n      ",
    "video_pixels": "1080p",
    "ram_size": "2GB RAM",
    "chipset": "MT8735",
    "battery_size": "3400mAh",
    "battery_type": "Li-Ion"
  }
}
```

## Search Phone
search for specific phone
endpoint ``/gsmarena/search/phone/:phone``, example ``/gsmarena/search/phone/nokia%208``

```json
  [
  {
    "name": "Nokia 8",
    "img": "https://cdn2.gsmarena.com/vv/bigpic/nokia-8-.jpg",
    "url": "nokia_8-8522.php",
    "description": "Nokia 8 Android smartphone. Announced Sep 2017. Features 5.3″ IPS LCD display, Snapdragon 835 chipset, Dual: 13 MP primary camera, 13 MP front camera, 3090 mAh battery, 128 GB storage, 6 GB RAM, IP54 certified, Corning Gorilla Glass 5."
  }
]
```

## TODO:
- [x] Get Reviews
- [x] Get Review
- [ ] Get News List
- [ ] Get News


