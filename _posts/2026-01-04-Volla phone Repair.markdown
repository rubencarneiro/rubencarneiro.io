---
title: "Volla X23 Phone Repair"
layout: post
date: 2026-01-03 23:41
tag: Repair Volla Phone
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla.png?raw=true)
headerImage: false
projects: false
blog: true
hidden: false # don't count this post in blog pagination
description: "How to revive a bricked Volla Phone x23"
category: blog
author: rubencarneiro
externalLink: false
---

<p align="center">
<img src="https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla.png?raw=true" />
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
# - So you bricked the Volla X23 and cant revert from custom rom to stock rom. I will help you.

&nbsp;
# How To fix it?



- Grab the files
- <a href="https://github.com/rubencarneiro/volla-x23/releases/download/1.0/boot.img">boot.img</a>
- <a href="https://github.com/rubencarneiro/volla-x23/releases/download/1.0/vendor_boot.img">vendor_boot.img</a>
- <a href="https://github.com/rubencarneiro/volla-x23/releases/download/1.0/volla-13.0-20240629-stable-vidofnir-signed.zip">flashable firmware</a>

&nbsp;

# Put the device in Fastboot

- in terminal do `fastboot flash boot.img`
- in terminal do `fastboot flash vendor_boot.img`

- reboot to recovery
- select apply update via adb
- in terminal do `adb -d sideload volla-13.0-20240629-stable-vidofnir-signed.zip `
- whait until is finish and clear all userdata and reboot. Its now fixed



# As Always please if you can donate. ;)

# <center>You Can donate by Paypal<center>
&nbsp;

<center>
<a href="https://paypal.me/rubencarneiro?locale.x=pt_PT" title="PayPal" onclick="javascript:window.open('https://paypal.me/rubencarneiro?locale.x=pt_PT','WIPaypal','toolbar=no, location=no, directories=no, status=no, menubar=no, scrollbars=yes, resizable=yes, width=1060, height=700'); return false;"><img src="https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-150px.png" border="0" alt="PayPal Logo"></a>