---
title: "Lil' Lamb"
image: "/lil-lamb-guts.jpg"
type: "page"
url: /lil-lamb
---

- *113 total LEDs (WS2812B)*
- *D1 Mini ESP32*
- *WLED Moonmodule v14.5.1-dev "Small Step"*
- *INMP441 I2S microphone*
- *Wire and solder*
- *Faux fur fabric*
- *hot glue*


I made this lil' lamb in preparation of the design and creation of the Pixel Lamb for *The Big Deal*- the 2023 manifestation of Wooly Fair. In reality, it didn't really serve as a stepping stone for the big one, but it did give us something fun to look at while we worked on Wooly Fair things. 

![Lil' Lamb guts](/images/lil-lamb-guts.jpg)

At some point after creating the physical layout I learned that I could create a custom map with .json. Once I figured that out, it started really looking nice. From there, I added an INMP441 I2S microphone, and to top it off, some hot glue to hold the electronics in place, and some faux fur fabric as the diffusion material.

I'm using a [sound-reactive fork](https://github.com/MoonModules/WLED-MM "link to WLED MoonModules Sound-Reactive software fork") of the WLED software to control the Lil' Lamb. 

![Lil' Lamb guts](/images/lil-lamb-back.jpg)

This lil' lamb will likely be auctioned off to some lucky bidder at an upcoming flocktion for [Wooly Fair](https://foley.works/wooly-fair/ "link to Wooly Fair page"). Below is a special section just for them. 

<div class="video-container">
  <video id="player" playsinline controls data-poster="/static/images/lil-lamb-back.jpg">
    <source src="/videos/lil-lamb3.mp4" type="video/mp4" />
  </video>
</div>

## Hello, new Lil' Lamb owner! 🐑

Congrats on your Lil' Lamb flocktion victory! You have great taste, and while I'll miss him, I'm thrilled this 'hypno-sheep' will find a place in your home. Below are some notes on the project which should help if you ever need to make an adjustment to software. 

### A Few Notes

- While you can always acccess the LED controls for your Lil' Lamb via IP address and a browser, I like the WLED phone app, and recommend that you use it. Once this is downloaded, you can search for your lil' guy, and add him as a device in your app. From there on out, all you need to do to change LED patterns, brightness, etc is to open your WLED app and click on your installation. I'll be happy to help walk you through this important first step.
- If you need to make an adjustment to or re-installation of the software running on the D1 Mini ESP32, all you need is a micro USB cord, a computer, and access to the back of the Lil' Lamb.
- There are a few websites where you can easily access various WLED software packages. I've found [this one](https://wled-install.github.io "Link to WLED Software installation website") to be the best, especially when it comes to sound-reactive offerings. You received your Lil' Lamb running the 'MoonMod' option at the bottom, for 4MB ESP32. 
- Simply plug in the micro USB cord to your computer with the D1 Mini ESP32 attached to it. Select the software you want, and install. 
- Once the installation is complete, you'll have the option to install the new software, or update the current WiFi settings on the current installation. Another option is to visit the URL of the device. Please note that accessing the UI for the WLED program via IP address is essentially the same as accessing it via the phone app. So if you prefer to not use apps and would like to access the controls via web page, simply bookmark the IP address. 
- When you visit the device settings, either via phone app or IP address, you can adjust important settings, such as your Wifi credentials. All other settings should not be touched, unless for some reason you decided to hack the hardware. 
- If you want to bring your Lil' Lamb to a new Wifi network, the process for updating the WiFi credentials is pretty easy. Plug in the Lil' Lamb in it's new spot, and as long as it's the only WLED installation on that network, you should be able to see a 'WLED-AP' network in your network list. Once you select it, you'll be brought to the interface where you can change the WiFi credentials to the credentials of the new network. After you enter them, select the new WiFi network on your phone, and your Lil' Lamb should now be accessable both via IP address, or with the WLED phone app. 
- Unlikely scenario, but if you decide to edit the LED layout of the Lil' Lamb, you'll be able to find the custom json mapping [here](https://github.com/yelof3/lil-lamb "link to lil' lamb WLED .json map"), and can edit it accordingly. 

