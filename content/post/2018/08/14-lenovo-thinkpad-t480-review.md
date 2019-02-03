---
title: Lenovo Thinkpad T480 Review
date: 2018-08-14
tags: ["hack", "work", "thinkpad", "t480", "lenovo"]
image: https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672177/IMG_20180713_112114_HDR.resized.jpg
---

**TLDR;** The Lenovo Thinkpad T480 has an amazing keyboard, a powerbridge system giving it a long battery life, a really crisp WQHD screen, and an almost fully compatible set of hardware with Ubuntu. The fingerprint reader doesn't work though, and it's a bit more bulky than the Dell XPS 13, especially with the external 72Wh battery.

<!--more-->

When Intel's new 8th gen CPUs were announced, I knew I was getting myself a new laptop to replace my Dell XPS 15 9560. I really appreciated the flexibility that the Dell offered me (I was able to replace the memory, the batteries, the SSD, and the wifi card) and I resolved that any new laptop purchase I made needs to be at least as hackable, if not more, than the Dell.

![My (relatively) old Dell XPS 15 9560](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672175/IMG_20180501_113059_HDR.resized.jpg)
*My (relatively) old Dell XPS 15 9560*

Maybe it was just a really fortunate coincidence, or it could be that Facebook was really listening in on my conversations, but I saw an advertisement for the Lenovo Thinkpad X1 Carbon 6th gen in my feed. I was somewhat familiar with the culture around the thinkpads, having bought a Thinkpad X60 many years ago (sadly I've lost that particular unit). The X1 Carbon was an ultrabook, and it meant that there are less upgrade options for me (especially on the RAM department) so poked around the site a bit more.

I got curious about the T480 and looked up more information about it. It wasn't as thin and light as the X1 Carbon, but it was portable enough. Plus, I've read that the [T series](https://en.wikipedia.org/wiki/ThinkPad_T_series) were the ones you bought if you needed to get actual work done (as opposed to looking hip and cool while working). After some time haggling with customer support and checking off hardware features, I finalized my order of my first Thinkpad after Lenovo bought the brand.

Here is [Notebookcheck's comprehensive review of the T480](https://www.notebookcheck.net/Lenovo-ThinkPad-T480-Core-i7-8650U-FHD-Laptop-Review.315574.0.html). They always do really good reviews, and they're my go-to site for any new hardware that comes up, so I decided I'll just highlight some sections that is unique to my usecase.

 My unit isn't exactly the same as their review unit, and here's the relevant buildout:

* Battery: 3cell 24Wh Front
* Battery 2: 6cell 72Wh Rear
* System Unit: T480 i5-8250U IG
* Camera: IR&HD Camera Mic
* AC Adapter and Power Cord: 65W USB-C 3Pin UK
* Processor: Intel Core i5-8250U MB
* Display: 14.0 WQHD IPS AG 300N
* System expansion slots: Smart Card Reader
* Graphic Card: Integrated Graphics
* Hard drive: 256GB SSD M.2 2280 NVMe OPAL2
* Keyboard Language: Backlit KYB ENG
* Total memory: 8GB DDR4 2400 SoDIMM
* Near Field Communication: NFC
* Pointing device: Fingerprint Reader w/NFC
* Preload OS: Windows 10 Home 64
* Display Panel: T480 WQHD NT IRCM MC NW PPS

Estimated Total: RM 5,116.00 MYR (about USD 1,250)

I chose the buildout specifically for my usecase as a software (mostly web) developer that uses Ubuntu as the preferred operating system:

* I took the 6cell 72Wh external battery for extra long computing without having to be near a power outlet.
* I didn't get the Nvidia MX 150 option. My Dell XPS 15 9560 had the Nvidia 1050 graphics card, and I've had a really terrible time getting the drivers (especially Optimus) working under Ubuntu. The issue is that if I don't get Optimus working, battery life really sucks. I figured it's not worth the hassle to get hardware made by company that's [openly hostile to GNU/Linux](https://drewdevault.com/2017/10/26/Fuck-you-nvidia.html) so I just opted to stay with the Intel integrated graphics solution, which is widely supported.
* I took the IR camera instead of the normal camera plus the ThinkShutter even though Ubuntu doesn't support Windows Hello. Here's hoping I'd be able to use it someday.
* I took the i5 instead of the i7 because for the 8th generation U series processors, the i5 is a quad-core multithreaded CPU just like the i7; the only difference being that the i7 was clocked higher than the i5. I don't play games and I won't be doing a lot of CPU intensive tasks on this laptop (I have my Clevo P650RSG for that) so I decided to save the money and use it for something else instead.
* I took the WQHD screen instead of the FHD with touchscreen. I find myself not using touch that much (judging from my experience with my Dell XPS 13 9343---I even disabled the touchscreen device at some point) so it wasn't any loss for me. The crispness of the display is amazing though, and the color accuracy was a lot better too.
* I got a smart card reader, which works perfectly with my E-residency card from Estonia.
* I took the NVMe SSD knowing that I would be replacing it later on with a cheaper and more spacious SATA SSD because I just wanted another NVMe stick.
* I took the least amount of memory possible with the system, as I had two sticks of 16GB DDR4 RAM from before prices skyrocketed.
* I took the NFC option which I haven't been able to get working under Ubuntu, but hey it's there just in case.
* Same with the finger print reader, which is also not yet supported.
* There wasn't any option to have an OS-less build so I just took the most basic version available (Windows 10 Home).

![The XPS 15 9560, Thinkpad T480, and XPS 13 9343 side by side](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672174/DSC3921.resized.jpg)
*The XPS 15 9560, Thinkpad T480, and XPS 13 9343 side by side*

Size-wise, it wasn't that much different from the Dell XPS 15 9560 even though it's a 14in laptop. This is because the T480 still maintains the somewhat thick (by today's standards) bezels, although not as thick as the Macbook Air 13. The external battery also raises the back of the unit a couple of centimeters, which I would like to think also benefits the airflow.

![The XPS 15 9560, Thinkpad T480, and XPS 13 9343 on top of each other](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672175/DSC3931.resized.jpg)
*The XPS 15 9560, Thinkpad T480, and XPS 13 9343 on top of each other*

Things I didn't really like, or initially had isues with about the T480:

* The trackpad had a bit more friction than I was used to. This is less of a problem now, because either I got used to the texture, or I've been wearing down the surface with my finger so it's not smoother. It was really rough, or much rougher than I was used to coming from the Dell XPS 15 9560, and I really missed the responsiveness from the Dell. It doesn't bother me as much nowadays, but sometimes when I fire up my Dell for old times' sake, I get reminded of the difference.
* The keyboard took getting used to. I was used to Apple external keyboards, and my favorite is still the Magic Keyboard with Numeric Numbad, and that means keyboards with far less travel than normal. Now that I've been using the Thinkpad keyboard for a couple of months now, I feel that it's way better than the Dell keyboard.

![Left Side Ports](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672174/DSC3932.resized.jpg)
*Left Side Ports*

Things I missed from the Dell XPS:

* The power led indicator on the side. I was used to checking the battery life of the laptop without having to open the device, and I missed that feature from the XPS series.
* The super thin bezels. I keep thinking that the T480 could have just as easily trimmed off a centimeter or two from its width had it opted to use thinner bezels.

![Right Side Ports](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672174/DSC3933.resized.jpg)
*Right Side Ports*

Things I loved about the T480:

* The port selection. I have USB-C (one of them Thunderbolt enabled), Gigabit Ethernet, an SD Card reader, and USB-A ports without needing to use a dongle. It's really convenient to have them built-in to the laptop, instead of having to remember to carry around adapters.
* USB-C Power Delivery support (aka charging). I really like USB-C not for the additional bandwidth it can support, but because of power delivery. I was able to survive a two month trip to Europe with only a single 65 watt USB-C charger with me. It can charge both of my cellphones (main and backup in case my daily driver gets stolen), my powerbank, and my laptop. I did have to bring an extra cable for my iPad Pro (which I charged off from my power bank), but imagine if the world just standardized on a single power interface?
* The clickable buttons. I don't use the nipple (aka trackpoint) but I really appreciate the clickable row of buttons just above the trackpad. It allows click-and-drag actions to be performed much more easily and accurately. The fact that it's above the trackpad was a bonus, because I can press CTRL-click with my left hand (pinky + thumb) without stretching too much; useful to feed my browser tab addiction.
* Power Bridge. I already get amazing battery life with the combination of the 24Wh and 72Wh batteries, but being able to swap out the external battery for another one means I can just bring an extra battery with me on trips and be able to use the laptop for a full day. If I need to be really thin and light (and I know I can get to a power outlet nearby, like in the office) I can just swap the bulky 72Wh battery with the thin 24Wh battery and enjoy the benefit of a thin and light ultrabook.
