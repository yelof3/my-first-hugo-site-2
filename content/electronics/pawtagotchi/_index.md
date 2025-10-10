---
title: "Pwnagotchi"
image: "/pawtagotchi.jpg"
type: "page"
url: /pwnagotchi
---

- *Raspberry Pi Zero 2W*
- *Waveshare 2.13inch e-Paper Hat E-Ink Display*
- *Pi Sugar 3 battery*

I found myself with an extra Pi Zero 2W, so why not build a cute lil’ wifi network handshake tool called the [Pwnagotchi](https://pwnagotchi.ai "link to pwnagotchi.ai"). All in all, apart from time taken to order and receive parts in the mail, this was a pretty quick project to get up and running. 

From that site:
## Pwnagotchi is an A2C-based “AI” powered by bettercap and running on a Raspberry Pi Zero W that learns from its surrounding WiFi environment in order to maximize the crackable WPA key material it captures (either through passive sniffing or by performing deauthentication and association attacks). This material is collected on disk as PCAP files containing any form of handshake supported by hashcat, including full and half WPA handshakes as well as PMKIDs.

I just completed this project! I found [this video guide](https://youtu.be/gyKT_mASSuc?si=hraGutKUQ6CO1G0l "Youtube video by Talking Sasquatch for setting up a Pwnagotchi]") by Talking Sasquatch to be quite helpful. A Reddit thread also helped me realize that the Waveshare I received with a V4 decal on it was in fact a V3.

After a quick adjustment on the config file to adjust the Waveshare version, I was off and running, capturing handshakes throughout the hood. I renamed mine Pawtagotchi, appropriately.

# Update
Pawtagotchi has surpassed 600 pwns. Another win for urban living. Here you can see the case I printed for my pwnagotchi, made with plant-based eco resin from Anycubic.

![pawtagotchi](/pawtagotchi.jpg)