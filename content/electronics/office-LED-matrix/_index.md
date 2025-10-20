---
title: "Office LED Matrix"
image: "/officeledmatrix.jpg"
type: "page"
url: /office-led-matrix
---

- *1,035 LEDs*
- *WS2812B RGB LED*
- *69 x 15*
- *D1 Mini ESP32*
- *INMP441 I2S Microphone*
- *Mean Well RSP-200-5 40a Power Supply*
- *Wire and solder*
- *1/8″ Frosted plexiglass diffusion panel*

![office-LED-matrix](/officeLEDmatrix.jpg)



I laid out most of the LEDs on this board during the beginning of the COVID-19 pandemic, probably sometime in late 2020. Due to placing my attention on other projects, this took a bit of time to finish, but I’m happy to say it’s finally finished in January 2025!

It has an improvement from the original sketch- sound reactivity! 

# Router Improvement
Past matrices had rather rudimentary frames and diffusion panels, typically using computer paper as the diffusion material. Worked nicely for smaller matrices, but this time around, I needed a better way to build the frame. 

A wood router was the answer! That allowed me to cut even grooves for the diffusion panel, so that it was able to just slide right into the frame. 

# Software Update
I started out with the 'standard' WLED sound reactive version. It worked well enough where I was able to tailor some patterns to my awkward 69x15 LED matrix, but it still really didn't compare to the paterns on the current non-sound-reactive WLED install. 

I did some searching, and saw a post indicating that the [WLED MoonModules](https://mm.kno.wled.ge "link to WLED MoonModules fork page") fork might be better with non-square matricies. I gave it an upload, reset my audio and data pin settings, as well as matrix dimensions, etc, and I was off and running. Overall, this sound reactive fork has been the best performer for my super-rectangle matrix, and I'm happy I spent a bit of time looking into another fork. 

