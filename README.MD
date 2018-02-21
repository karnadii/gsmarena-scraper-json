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
        },
        {
          "name": "2G bands",
          "value": "GSM 850 / 900 / 1800 / 1900 - SIM 1 & SIM 2"
        },
        {
          "name": "3G bands",
          "value": "HSDPA 850 / 1900 / 2100 "
        },
        {
          "name": "4G bands",
          "value": "LTE band 1(2100), 3(1800), 7(2600), 8(900), 20(800)"
        },
        {
          "name": " ",
          "value": "LTE band 3(1800), 7(2600), 8(900), 28(700)"
        },
        {
          "name": "Speed",
          "value": "HSPA 42.2/11.5 Mbps, LTE Cat4 150/50 Mbps"
        },
        {
          "name": "GPRS",
          "value": "Yes"
        },
        {
          "name": "EDGE",
          "value": "Yes"
        }
      ]
    },
    {
      "category": "Launch",
      "specs": [
        {
          "name": "Announced",
          "value": "2016, August"
        },
        {
          "name": "Status",
          "value": "Available. Released 2016, October"
        }
      ]
    },
    {
      "category": "Body",
      "specs": [
        {
          "name": "Dimensions",
          "value": "191.7 x 101 x 9.4 mm (7.55 x 3.98 x 0.37 in)"
        },
        {
          "name": "Weight",
          "value": "260 g (9.17 oz)"
        },
        {
          "name": "SIM",
          "value": "Dual SIM (Micro-SIM/Nano-SIM)"
        }
      ]
    },
    {
      "category": "Display",
      "specs": [
        {
          "name": "Type",
          "value": "IPS LCD capacitive touchscreen, 16M colors"
        },
        {
          "name": "Size",
          "value": "7.0 inches, 135.1 cm2 (~69.8% screen-to-body ratio)"
        },
        {
          "name": "Resolution",
          "value": "720 x 1280 pixels, 16:9 ratio (~210 ppi density)"
        },
        {
          "name": "Multitouch",
          "value": "Yes"
        }
      ]
    },
    {
      "category": "Platform",
      "specs": [
        {
          "name": "OS",
          "value": "Android 6.0 (Marshmallow)"
        },
        {
          "name": "Chipset",
          "value": "Mediatek MT8735"
        },
        {
          "name": "CPU",
          "value": "Quad-core 1.3 GHz Cortex-A53"
        },
        {
          "name": "GPU",
          "value": "Mali-T720MP2"
        }
      ]
    },
    {
      "category": "Memory",
      "specs": [
        {
          "name": "Card slot",
          "value": "microSD, up to 128 GB (dedicated slot)"
        },
        {
          "name": "Internal",
          "value": "16/32 GB, 2 GB RAM"
        }
      ]
    },
    {
      "category": "Camera",
      "specs": [
        {
          "name": "Primary",
          "value": "13 MP, autofocus"
        },
        {
          "name": "Features",
          "value": "Geo-tagging, touch focus, face detection, HDR, panorama"
        },
        {
          "name": "Video",
          "value": "1080p@30fps"
        },
        {
          "name": "Secondary",
          "value": "2 MP, 720p"
        }
      ]
    },
    {
      "category": "Sound",
      "specs": [
        {
          "name": "Alert types",
          "value": "Vibration; MP3, WAV ringtones"
        },
        {
          "name": "Loudspeaker ",
          "value": "Yes"
        },
        {
          "name": "3.5mm jack ",
          "value": "Yes"
        },
        {
          "name": " ",
          "value": "- DTS HD sound\n"
        }
      ]
    },
    {
      "category": "Comms",
      "specs": [
        {
          "name": "WLAN",
          "value": "Wi-Fi 802.11 a/b/g/n, Wi-Fi Direct, hotspot"
        },
        {
          "name": "Bluetooth",
          "value": "4.0, A2DP"
        },
        {
          "name": "GPS",
          "value": "Yes, with A-GPS, GLONASS"
        },
        {
          "name": "Radio",
          "value": "FM radio"
        },
        {
          "name": "USB",
          "value": "microUSB 2.0"
        }
      ]
    },
    {
      "category": "Features",
      "specs": [
        {
          "name": "Sensors",
          "value": "Accelerometer, proximity"
        },
        {
          "name": "Messaging",
          "value": "SMS(threaded view), MMS, Email, Push Mail, IM"
        },
        {
          "name": "Browser",
          "value": "HTML"
        },
        {
          "name": " ",
          "value": "- MP4/H.264 player\n- MP3/WAV/eAAC+/Flac player\n- Photo/video editor\n- Document viewer"
        }
      ]
    },
    {
      "category": "Battery",
      "specs": [
        {
          "name": " ",
          "value": "Non-removable Li-Ion 3400 mAh battery (12.92 Wh)"
        },
        {
          "name": "Talk time",
          "value": "Up to 9 h (multimedia)"
        }
      ]
    },
    {
      "category": "Misc",
      "specs": [
        {
          "name": "Colors",
          "value": "Black"
        },
        {
          "name": "Price",
          "value": "About 170 EUR"
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

TODO:
- [x] Get Reviews
- [x] Get Review
- [ ] Get News List
- [ ] Get News


