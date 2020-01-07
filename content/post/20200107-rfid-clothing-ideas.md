+++
title = "RFID ideas to manage my clothes"
date = "2020-01-07T10:00:00+02:00"
tags = ["diy","rfid","esp32","arduino"]
draft = false
+++

This post is basically the result of an idea that came to my mind. I researched about it for a couple of hours, and here are my conclusions.

The original idea was controlling clother on my wardrobe or house. I want to get RFID tags as cheap and as small as possible, to use it on all my garments, and read them later (desirable read range larger than 25-30cm) to passively position them indoor (to see if they are on the wash drum, or in my closet, or drying). Turns out that is the same technology used on warehouses to track goods. I need wash-resistant tags, so I must be careful picking paper-based tags.

Note that I can (but **don't want to**) use the following approaches:
- Tracking items manually
- Tracking items with the camera (barcode-based solution)
- Tracking items with HF RFID (e.g. NFC), using a reader on the wall, or using my smartphone
but I want to go a step further, thus needing more RF range.

For getting the desired range, I probably need to work in the UHF band (solutions found on the HF band are usually on the range of the low-single-digit centimeters). So UHF then.

Tech behind some cashier-less stores (e.g. Decathlon) could also be similar to what I need. Regarding the exact Decathlon case, it seems that they are using a very ad-hoc solution (a smart decision for them, but not suitable for me).

Shortly, the way to go seems to involve some form of ISO 18000-6C standard (EPC Gen 2 Class 1 UHF). In Europe, uses (aprox.) 868Mhz, and 960Mhz in America. The standard is suited to work with both frequencies.

Items I found:

- [Tags (about 8€ for 50 of them)](https://es.aliexpress.com/item/32772873727.html)
- [Readers, about 50€ (this one is USB-based. Perhaps, looking to RPi/Arduino/ESP32 RS485 would be better)](https://es.aliexpress.com/item/32801951489.html)

So, this idea remains on-hold, due to high pricing. Worth the research, though.

Happy hacking!