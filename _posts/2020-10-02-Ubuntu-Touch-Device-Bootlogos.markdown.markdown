---
title: "Ubuntu Touch Custom Device Bootlogos"
layout: post
date: 2020-10-02 21:58
tag: Ubuntu Logos
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/screenshots/ubuntu_touch.jpg?raw=true)
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "Making bootlogo to varius devices to use on Ubuntu touch devices."
category: project
author: rubencarneiro
externalLink: false
---

![Screenshot](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/screenshots/ubuntu_touch.jpg?raw=true)

---
What are bootlogos?
---
Bootlogos that bright vendor logo that sometimes almost blind you in the dark, yeah that thing.

OnePlus One         |  OnePlus One 3/3T
:-------------------------:|:-------------------------:
![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/oneplusone.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>  |  ![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/oneplus3.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>


Nexus 5        |  Fairphone 2
:-------------------------:|:-------------------------:
![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/Nexus-5.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>  |  ![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/fairphone2.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>

Bq E5        |  BQ E4.5
:-------------------------:|:-------------------------:
![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/bqe5.jpg?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>  |  ![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/bqe45.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>

BQ M10HD        |  BQ M10FHD
:-------------------------:|:-------------------------:
![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/bqm10.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>  |  ![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/bqm10fhd.png?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>


Meizu MX4        |  Volla Phone
:-------------------------:|:-------------------------:
![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/meizumx4.jpg?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>  |  ![](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/bootlogos/volla.jpg?raw=true)<a href="https://open-store.io/app/chatter.ruben-carneiro" rel="some text">![Foo](https://open-store.io/badges/en_US.png)</a>


Nexus 5
=======
**How to flash**:

- Reboot device to fastboot
- `fastboot flash imgdata imgdata.img`


Fairphone 2
===========
**How to flash**:

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash splash splash.img`


Meizu MX4
=========
**How to flash**:

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash logo logo.bin`


BQ E4.5
=========
**How to flash**

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash logo logo.bin`


BQ E5
=========
**How to flash**

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash logo logo.bin`


BQ M10HD
=========
**How to flash**

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash logo logo.bin`


BQ M10FHD
=========
**How to flash**

- Reboot device to fastboot
- In a terminal and do:
- `fastboot flash logo logo.bin`


OnePlus One
=========
**How to flash**

- Reboot device to fastboot
- In a terminal do:
- `fastboot flash LOGO logo.bin`

OnePlus One 3/3T
=========
**How to flash**

- Reboot device to fastboot
- In a terminal do:
- `fastboot flash LOGO logo.bin`
- for some reason some people are unable to flash trough fastboot "FAILED (remote: Partition flashing is not allowed)"
- Use the update-zip and flash trough recovery: https://drive.google.com/file/d/1MBA7yJREcnQ_Pg8D3_cY_VNry-L4_aSc/view

Volla Phone
=========
**How to flash**

- Reboot device to fastboot
- In a terminal do:
- `fastboot flash logo logo.bin`

Bq Aquaris U Plus
=========
**How to flash**

- Reboot device to fastboot
- In a terminal do:
- `fastboot flash splash splash.img`

As an independent porter i get no income for this, i do it for pleasure and for the community, it takes time,research and a lot of patience so if you can donate.
Also follow my channel on youtube a give a like they are only a few videos but maybe i can make more in time.

# <center>Donate<center>
<center><table border="0" cellpadding="10" cellspacing="0"
align="center"><tbody><tr><td align="center"></td></tr><tr><td align="center"><a href="https://paypal.me/rubencarneiro?locale.x=pt_PT" title="PayPal" onclick="javascript:window.open('https://paypal.me/rubencarneiro?locale.x=pt_PT','WIPaypal','toolbar=no, location=no, directories=no, status=no, menubar=no, scrollbars=yes, resizable=yes, width=1060, height=700'); return false;"><img src="https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-150px.png" border="0" alt="PayPal Logo" /></a></td></tr></tbody></table>