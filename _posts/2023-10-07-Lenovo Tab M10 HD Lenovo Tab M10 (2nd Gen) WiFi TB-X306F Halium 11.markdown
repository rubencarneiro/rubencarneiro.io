---
title: "Lenovo Tab M10 (2nd Gen) WiFi TB-X306F"
layout: post
date: 2023-10-07 19:49
tag: Lenovo M10 HD Port
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/x306f/x306f.png?raw=true)
headerImage: false
projects: true
blog: true
hidden: false # don't count this post in blog pagination
description: "Status of port"
category: project
author: rubencarneiro
externalLink: false
---

<p align="center">
<img src="https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/x306f/x306f.png?raw=true" />
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

Lenovo Tab M10 HD (amar_row_wifi) specs
==========================================

## Halium 11 based

# Status

- [X] Recovery
- [X] Boot
- [X] Bluetooth
- [X] Camera Fotos and Video Recording
- [x] GPS
- [X] Audio works
- [X] Bluetooth Audio
- [X] Waydroid
- [X] MTP
- [X] ADB
- [X] SSH
- [X] Online charge
- [X] Offline Charge
- [X] Wifi
- [X] SDCard
- [X] Wireless display ( Broken cannects and disconnects sometimes image will cast )
- [X] Manual Brightness Works
- [X] Hardware video playback
- [X] Rotation
- [X] Proximity sensor
- [X] Virtualization
- [X] GPU
- [X] Lightsensor
- [X] Proximity sensor
- [X] Automatic brightness
- [X] Hotspot
- [X] Airplane Mode

## Install:

- Download The latest devel-flashable-focal image from latest CI builds
https://gitlab.com/uports/h10/lenovo-m10-hd/lenovo-m10-hd/-/pipelines

- Flash the Ubuntu boot.img:
``fastboot flash boot ./boot.img ``

- Download [vbmeta.img](https://github.com/rubencarneiro/amar_row_wifi/releases/download/1.0/vbmeta.img)
``fastboot --disable-verification flash vbmeta ./vbmeta.img ``
- Reboot to fastboot
``fastboot reboot fastboot``
- Format userdata
``fastboot format:ext4 userdata``
- Delete product logical partition
``fastboot delete-logical-partition product``
- Resise system partition
``fastboot resize-logical-partition system 3978565472``
- Flash Ubuntu Rootfs:
`` fastboot flash system ./ubuntu.img``

## <center>As Always please if you can donate to my paypal. ;)</center>


