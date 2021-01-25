---
title: "Volla Phone Repair"
layout: post
date: 2021-01-25 21:21
tag: Repair Volla Phone
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/brand/bootlogobrand.png?raw=true)
headerImage: false
projects: false
blog: true
hidden: false # don't count this post in blog pagination
description: "How to revive a dead Volla Phone"
category: blog
author: rubencarneiro
externalLink: false
---

![Screenshot](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla.png?raw=true)

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

 ---
So how did i bricked my Volla?
---
- Well it was very easy to brick i just commit a stupid error of flashing a custom rom made to GS290, is the same phone right?, Maybe not.
Look this is my experience, and my experience only, you may have other methods this was how it happened to me and how i fixet.
As i flashed i had to install a custom recovery TWRP for GS290 i Installed the rom and my device keeps rebooting everytime i tried to watch a Youtube video so i decided lets go back to Volla OS or Ubuntu Touch.
Well things just gone wrong from there as tried to reflash my stock recovery for volla my phone went dead, not turning on. Damm i brick my phone let try lsusb in terminal " Bus 001 Device 058: ID 0e8d:0003 MediaTek Inc. MT6227 phone" that was wrong.
So  at this time my phone is in Mediatek mode for flash or preloader.
My phone is just a black screen do not turn on does nothing.

 ---
How To fix it?
---

- Grab Spflashtool
- <a href="https://spflashtool.com/download/SP_Flash_Tool-5.1916_Linux.zip">Linux</a>
- <a href="https://spflashtool.com/download/SP_Flash_Tool_v5.1924_Win.zip">Windows</a>

- When using linux cd spflashtool folder then
- `chmod a+x flash_tool flash_tool.sh`
- run as superuser

 ---
Files that you need
---
- <a href="https://volla.tech/filedump/ubuntu-touch-yggdrasil-ota15-flashtool.zip">Volla ubuntu Touch OTA-15 flashtool zip</a>

- extract the file and open spflashtool as sudo
- call the scatter file inside te extracted folder "MT6763_Android_scatter.txt" and select firmware Update as the picture below.

![Screenshot](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/spflashtool.png?raw=true)

- Press Download 

- Connect your type-c cable if it dont detect as first time remove and reconnect the cable.

- Wait until flash, once it finish now you can turn your device on and acess recovery and fastboot etc.

- Go to fastboot and do the following command `fastboot flash unlock` this will unlock the boot loader and you be able to flash a custom or original recovery. I suggest you to use stock recovery.


