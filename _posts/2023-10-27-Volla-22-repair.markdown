---
title: "Volla 22 Phone Repair"
layout: post
date: 2023-10-27 22:21
tag: Repair Volla 22 Phone
image: (https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/volla.png?raw=true)
headerImage: false
projects: false
blog: true
hidden: false # don't count this post in blog pagination
description: "How to revive a dead Volla 22 Phone"
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

# Necessary steps

- Grab Spflashtool
- <a href="https://spflashtool.com/download/SP_Flash_Tool-5.1916_Linux.zip">Linux</a>
- <a href="https://spflashtool.com/download/SP_Flash_Tool_v5.1924_Win.zip">Windows</a>

- When using linux cd spflashtool folder then
- `chmod a+x flash_tool flash_tool.sh`
- run as superuser

&nbsp;

# Files that you need

- <a href="https://volla.tech/filedump/vollaos/volla-11.1-20221017-stable-SPFLASH-mimameid.zip">Volla 22 stock firmware</a>

- extract the file and open spflashtool as sudo
- call the scatter file inside te extracted folder "MT6768_Android_scatter.txt" and select firmware Update as the picture below.

![Screenshot](https://github.com/rubencarneiro/rubencarneiro.io/blob/main/assets/images/devices/volla/spflashtool.png?raw=true)

- Press Download 

- Connect your type-c cable if it dont detect as first time remove and reconnect the cable.

- Wait until flash, once it finish now you can turn your device on and you should be booting to stock Android 11 Volla OS.


### <center> As Always please if you can donate. ;)<center>
