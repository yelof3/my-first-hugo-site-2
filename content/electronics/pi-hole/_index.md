---
title: "Pi-Hole"
image: "/pi-hole.jpg"
type: "page"
url: /pi-hole
---

- *Raspberry Pi Zero 2W*
- *MicroSD Card*
- *Raspberry Pi Zero Case*
- *Raspberry Pi OS*
- *Pi-hole software*

This Pi-Hole project can be done in as little as 15 minutes, or if you have an old Netgear router like I had, maybe a few days. It has no fancy appearance, but has a huge impact in the home. Not only will you rid yourself of most advertising on your network devices, but you’ll also be able to take a closer look at the details of your network traffic, and speed up your overall network as well!

![pi-hole](/pi-hole.jpg)

The steps are fairly straight forward. 

- Install Raspberry Pi OS (or your OS of choice) on the Raspberry Pi. I used the 32-bit version.
- SSH into the Pi, run update and upgrade
- Install Pi-Hole with the following command:
- curl -sSL https://install.pi-hole.net | bash
- From there, answer a few easy questions, and you’ll then have Pi-Hole installed on your Pi. Visit the Pi-Hole website for official docs, links, etc.
- Decide the best method for incorporating your Pi-Hole device into your network as the DNS server. This doc from Pi-Hole covers the options nicely. 

# Pi-Hole Router DNS Issues
The router that I had been using for the last 12 years or so is the Netgear 450N, CG3000Dv2. Old, but it’s done the trick…up until this project, when I needed to be able to control DNS settings. From what I’ve read on the internet, the ISP where I purchased the router from, Cox, likely put firmware on it that prohibits the adjustment of DNS settings.

Off I went to Craigslist/Facebook Marketplace, and found myself a nice little Allesis SBG10 Surfboard router/modem. Changing settings on the Allesis has been a breeze, and since implementing that into my network and placing the correct DNS settings on the admin page I’ve had great luck with the Pi-Hole!

![pi-hole](/pi-hole-admin.png)

I must say, there was a feeling of power after watching a whole movie free of ads on Tubi, a movie platform that is laden with ads.

# ISP Rep Beef
One fun part of this project was after I gathered that I would need to call Cox to have them assign my new router/modem to my account. 

I researched their online docs regarding modem compatibility, but upon calling them the rep said that my new modem was not compatible. I told them that it was listed on their official compatibility list, but he assured me that it wasn’t compatible, and said that since I had the list in front of me, I should do the research on which modems would work. Ha!

I ended up getting off the call and registering the device on their website in 5 minutes. 



