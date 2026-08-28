---
title: "Bjorn"
image: "/images/bjorncyberviking.png"
type: "page"
description: "I recently installed Bjorn on an extra Pi Zero W I had lying around. Here's what happened."
url: /bjorn
---

- *Raspberry Pi Zero W*
- *Waveshare 2.13inch e-Paper Hat E-Ink Display, V4*
- *Micro SD Card*
- *3D Printed Case*

I found myself with (another) extra Pi Zero W, so why not build a cute lil’ pentesting tool called [Bjorn](https://codeberg.org/yelof/Bjorn_Again "link to my Bjorn project on Codeberg"). 

From the README:
> Bjorn is a powerful tool designed to perform comprehensive network scanning, vulnerability assessment, and data ex-filtration. Its modular design and extensive configuration options allow for flexible and targeted operations. By combining different actions and orchestrating them intelligently, Bjorn can provide valuable insights into network security and help identify and mitigate potential risks.

![Bjorn Cyberviking](/images/bjorncyberviking.png)

After unpacking the software, I had to take care of a few particulars for my specific setup, including:
- *deal with SSH key issues on my Mac, where I was SSHing to the Pi from*
- *Figured out why my keyboard wasn't being recognized as a USB host device. Bjorn's installation configured the Pi Zero's single USB data port for USB gadget mode: dwc2 + g_ether. That made the Pi treat the USB port as a network/device connection rather than a normal USB host. I then disabled usb-gadget.service, removed g_ether from the boot command line, explicitly configured the USB controller for host mode with: dtoverlay=dwc2,dr_mode=host*
- *Another installation issue: ModuleNotFoundError: No module named 'rich'. Repaired missing dependencies.*
- *pandas==2.2.3 downloads on a Pi Zero W and then fails the requirements-file hash check*
- *Downloaded 5 Python dependencies that failed with the panda hash check- sqlalchemy, paramiko, smb (provided by pysmb), netifaces, and pymysql*


