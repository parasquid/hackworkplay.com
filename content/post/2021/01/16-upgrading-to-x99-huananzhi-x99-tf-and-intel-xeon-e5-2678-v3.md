---
title: "Upgrading to X99: Huananzhi X99-TF and Intel Xeon E5-2678 v3"
date: 2021-01-16
tags: ["hack", "work", "x99", "intel", "unraid"]
image: https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1610881129/hackworkplay/IMG_20210109_183441.jpg
---
I've been running an i7 3770 (purchased in 2013 from a colleague) as my NAS using [unRAID](https://unraid.net/). Since it's unRAID, I'm not limited to just using it as a NAS but also as a torrent client (for downloading linux distros of course), plex media server, and various dockers for postgres and mysql databases, calibre, syncthing, etc. I'm also running a couple of VMs that I use as my workspace for my work projects through vscode remote.

<!--more-->

![picture of my old server](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1610882372/IMG_20201205_161905.jpg)
*my old i7 3770 server inside a Fractal Design 7 case in storage layout*

With the lockdowns in place forcing everyone to work from home, I thought it would be a good time for a hardware upgrade. Apparently many others thought the same, which caused hardware (like the new Zen 3 Ryzen cpus and nVidia 3000 series graphics cards) prices to either skyrocket or the hardware themselves to just plainly be unavailable.

While checking out online shops for possible deals on current-gen hardware, I happened to be recommended a new seller's products: an [x99 motherboard by Huananzhi](http://www.huananzhi.com/html/1/184/185/362.html#drivers) and an [E5-2678 v3 Intel Xeon cpu](https://www.cpu-world.com/CPUs/Xeon/Intel-Xeon%20E5-2678%20v3.html) combo for around RM900MYR (around $250USD).

![picture of a motherboard](https://res.cloudinary.com/psqd/image/upload/v1610883758/Hd65682309cbb469b8f53e654d2062d6c6.webp)
*picture taken from the online store*

The [motherboard and cpu combo](https://psqd.pw/x99-combo) was interesting because it can take both DDR3 and DDR4 memory. Apparently the cpu is not an official part, and was custom made for a few large companies during the time when DDR4 was new and not readily available; having a cpu support both DDR3 and DDR4 allows the companies to eventually upgrade to DDR4 without having to purchase new cpus.

Since the i7 3770 system I had was using DDR3, I thought this was quite advantageous for me as well; I can use my current DDR3 memory with a good upgrade route for eventually getting a modern system on DDR4 without having to spend on the hardware all at once. I can for example buy some DDR4 memory first and replace the DDR3, then get a new cpu and motherboard when the hardware prices become much more reasonable.

I did a bit of research, and the best review I've seen for the motherboard comes from a youtube channel named Miyconst. Below is his video review:

{{<youtube ctuOXMLATW4>}}

I thought that a 12-core/24-thread system with 40 pcie lanes is quite a good proxy for an eventual Ryzen 3900x/X570 combo system I'm planning for in the future, so I ended up buying the mobo-cpu package and set up the whole thing.

Everything worked well after assembly. I reused my DDR3 memory from the old i7 3770 as planned, and unRAID was as simple to migrate as just plugging in the USB thumbdrive from one system to the next.

![screenshot of the unraid dashboard](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1610882719/Screenshot_2021-01-03_at_1.22.45_AM.png)
*unRAID conveniently just picked up everything from where it left off; except now it has more cores available*

I can now assign more cores to my Ubuntu work VM to make development faster, and managming the server just feels a lot snappier. The only downside is the slight increase in power consumption (an extra 20 watts), but I felt this was a worthy investment, with good upgrade potential.

-----

Affiliate links:

* {{< open_links_in_target_blank "https://psqd.pw/x99-combo" >}}
