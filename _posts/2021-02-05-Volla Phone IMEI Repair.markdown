---
title: "Volla Phone IMEI Repair"
layout: post
date: 2021-02-05 21:07
tag: Repair Volla Phone IMEIS
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla2.png?raw=true)
headerImage: false
projects: false
blog: true
hidden: false # don't count this post in blog pagination
description: "How To Retrieve Volla Phone Imeis"
category: blog
author: rubencarneiro
externalLink: false
---

<p align="center">
<img src="https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla2.png?raw=true" />
</p>

# Disclaimer
<pre class="alt2 " dir="ltr" style="
		margin: 0px;
		padding: 5px;
		border: 1px inset;
		width: 100%;
		height: 210px;
		text-align: left;
		overflow: auto">#include &lt;std_disclaimer.h&gt;

/*
 * Your warranty is now void.
 *
 * I am not responsible for bricked devices, dead SD cards,
 * thermonuclear war, or you getting fired because the alarm app failed. Please
 * do some research if you have any concerns about features included in this ROM
 * before flashing it! YOU are choosing to make these modifications, and if
 * you point the finger at us for messing up your device, we will laugh at you.
 * Use at your Own Risk.
 *
 */</pre>

&nbsp;

# Lost IMEI's after Bricked Volla Phone
- If you dont Know how did i bricked my Volla Phone and unbricked i sugest you go to page <a href="https://rubencarneiro.github.io/rubencarneiro.io//Volla-phone-Repair/">Volla Phone Repair</a>

- Now After that i lost my Imeis and serial and part of the problem became part of the solution and heres how i recover it.

- Also my fingerprint reader dont work onVolla Roms and Ubuntu Touch, but works fine with the GS290 Firmware, hopelly Volla will update their firmware to android 10 and that will be fixed.

&nbsp;
# Get the files you need?

- <a href="https://build.lolinet.com/file/lineage/GS290/lineage-17.1-20210109-EXPERIMENTAL-GS290.zip">Lineage os 17.1 for GS290</a> As i said this was part of the problem but also was the solution so thanks to Erfan Abdi on telegram roup.
- <a href="https://build.lolinet.com/file/twrp/GS290/android-9.0/twrp-3.5.0-21-GS290.img">GS290 TWRP for Android 9.0 based</a> - You need to flash this one since your Volla Is based on android 9.0
- <a href="https://drive.google.com/file/d/129SBT1Vy5DzQAa-oJp_5g9vuP_IJtG-q/view?usp=sharing">GS290 Stock Rom Android 10 Based</a> Thanks to El Hundo in Telegram.

- <a href="https://build.lolinet.com/file/twrp/GS290/android-10.0/twrp-3.5.0-35-GS290.img">GS290 TWRP for Android 10 based</a> - You will flash this after flashing stock rom.

- <a href="https://spflashtool.com/download/SP_Flash_Tool-5.1916_Linux.zip">SPFLASHTOOL</a>


&nbsp;

# How To

- First flash the GS290 TWRP Android 9.0 based `fastboot flash recovery twrp-3.5.0-21-GS290.img`

- Now reboot to recovery and wipe all and reboot to recovery again and copy inside the .
- Now we will install Lineage OS 17.1 lineage-17.1-20210109-EXPERIMENTAL-GS290.zip

- After install reboot the system, go settings about and enable developer mode, go developer mode and enable advanced reboot or restart. now push power button and select reboot to bootloader.

- No flash GS290 TWRP Android 10 based `fastboot flash recovery twrp-3.5.0-35-GS290.img`

- Reboot again to recovery. Now on your computer do `adb shell`
- And the following commands:

- `mkdir /mnt/vendor/nvdata`

- `mount /dev/block/by-name/nvdata /mnt/vendor/nvdata`

- `restorecon -R /mnt/vendor/nvdata/ -v`

- `umount /mnt/vendor/nvdata && sync && reboot`

This commands where provide by Marc Aurel in Telegram official group <a href="https://t.me/hello_volla">Volla Group</a>

- Now extract the GS290 Stock Rom Android 10 Based and copy to your device the system.img vendor.img boot.img

- On TWRP go to Install and select Images and then select system.img and restore to system, boot.img to boot and vendor.img to vendor after install wipe factory reset and restart the phone.

- For some reason the phone will have FRP google Account to remove use the scatter inside the stock rom zip with spflash tools.

- Go to Format/ Manual Format and enter the Begin Address: 0x3888000 and the Format Lenght : 0x100000

![Screenshot](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/spflashtool2.png?raw=true)

- Turn the Phone down Click on Start in spflashtool and connect the cable to the phone once OK appers disconnect the cable and boot the phone, the google account was now removed, after initil setep you will notice that will ask you to enter a code + Fingerprint yes fingerprint is working,

- After Initial setup go to about the the phone and confirm that you now have the IMEIS.

# Whats next?

- Now you can flash you Ubuntu touch firmware
- <a href="https://volla.tech/filedump/ubuntu-touch-yggdrasil-ota15-flashtool.zip">Volla ubuntu Touch OTA-15 flashtool zip</a> Using spflash Tool

If You Want to Install Volla OS first unlock bootloader with the command:

- `fastboot flashing unlock`
- And flash stock recovery  <a href="https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/downloads/volla/stock_recovery.img?raw=true">Stock Recovery</a>

- Reboot to recovert select apply update trought adb

- Download Volla OS Firmware <a href="https://ota.volla.tech/builds/volla-9.0-20201019-nightly-k63v2_64_bsp-signed.zip">Volla OS</a>

Now do the command:
- `adb sideload volla-9.0-20201019-nightly-k63v2_64_bsp-signed.zip`
- After do Factory reset and reboot the device.

-If All go right Your phone is back again with Imeis

# Backup Partitions Using SPFlashTool
<iframe width="1252" height="704" src="https://www.youtube.com/embed/9QMq4RADon8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


&nbsp;

# Support

- I really hope that this will help you to fix your Volla Phone.
- I strongly encourage you to make a backup of your NVRAM parition Using SPflashtool and persist partition, so you can easy restore if anything happens to your device.

&nbsp;

# As Always please if you can donate to my paypal. ;)

# <center>You Can also donate by Crypto<center>
&nbsp;

[![Donate with Litecoin](https://en.cryptobadges.io/badge/micro/LdBPTusxmSoZ79x6oWd1864T6Q3afucay5)](https://en.cryptobadges.io/donate/LdBPTusxmSoZ79x6oWd1864T6Q3afucay5) [![Donate with Ethereum](https://en.cryptobadges.io/badge/micro/0xbac735b0918290451adddfbf1d4391658380c950)](https://en.cryptobadges.io/donate/0xbac735b0918290451adddfbf1d4391658380c950) [![Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/3Ef6fEm6fwcXHzuHQP3dHYeUF1Ftoveuwp)](https://en.cryptobadges.io/donate/3Ef6fEm6fwcXHzuHQP3dHYeUF1Ftoveuwp)
