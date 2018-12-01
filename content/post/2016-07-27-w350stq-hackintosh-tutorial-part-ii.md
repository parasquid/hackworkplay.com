---
title: W350STQ Hackintosh Tutorial Part II
date: 2016-07-27
tags: ["hack", "hackintosh", "illegear re-15 (aka clevo w350stq)"]
image: https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672166/DSC1481.resized.jpg
---

The wifi module I ordered from AliExpress [<small>affiliate link</small>](http://s.click.aliexpress.com/e/A2fqvVFEE) has finally arrived! Since this wifi module is the exact same chipset from Apple's Airport Extreme, MacOS should be able to immediately detect and use the module without any kexts or DSDT edits.
<!--more-->

Before opening up the covers and installing the wifi module, the laptop needs to be shutdown first and its battery removed. There's a small lock switch that needs to be pushed to unlocked, and the battery pops up when pushing the battery slider switch.

![Remove the Batteries](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672171/DSC1489.resized.jpg)
*safety first: always remove the battery when opening the computer*

The next step is to remove the grill at the top of the keyboard. You can use a flathead screw driver or anything thin and sturdy to pry open the grill starting from the left side. You will then be able to see five Philips screws that secures the keyboard to the chassis.

![Using a screwdriver to pop the grill cover](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672170/DSC1488.resized.jpg)
*you can use a screwdriver, or any flat sturdy tool to pop the grill cover open*

![Grill cover removed](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672171/DSC1487.resized.jpg)
*the grill cover should come completely off*

One thing you'll need to be very careful of is the keyboard ribbon cable. The cable attaches near the center of the keybaord, and it's tempting to just lift the keyboard away after the five screws have been removed. Remember, **lift the keyboard gently up and then turn it upside down** so you don't damage the ribbon cable.

![Keyboard Rainbow Cable](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672169/DSC1486.resized.jpg)
*be careful when trying to lift up the keyboard as the rainbow cable might hitch and be broken; lift the keyboard assembly slowly*

You should now be able to see where the old half-mini PCI-E card is at. This module (that's not compatible with MacOS) will be replaced with the new one (that's compatible with MacOS).

![Wifi modules](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672167/DSC1482.resized.jpg)
*the old module, and the new*

First, remove the screw that secures the wifi module to the motherboard. Then remove the two antennas; you might need to use a small screwdriver to pry the antenna from the wifi module. Don't force the antenna or pull it away; you might damage the connectors.

![Keyboard Rainbow Cable](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672168/DSC1483.resized.jpg)
*antennas removed*

At this point it's now just a matter of replacing the old wifi module with the new one. The antennas will have to go back the same way, and a screw is needed to secure the wifi module into the motherboard.

![Keyboard Rainbow Cable](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672168/DSC1484.resized.jpg)
*et voila! just need a screw to secure the module and we're done*

Boot up the computer, and it works! No drivers, no kexts, no DSDT edits, no more tethering. The hackintosh is finally portable and mobile :)

![Keyboard Rainbow Cable](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672171/DSC1490.resized.jpg)
*wifi works the minute I boot the hackintosh*

The only issue with this wifi module is that it doesn't support bluetooth. Then again, BT isn't really something that is important right now; the wireless mice that I use from Logitech use their own tranceivers and are a lot more compatible with my systems anyway.

I purchased the [wifi module](http://s.click.aliexpress.com/e/A2fqvVFEE) from AliExpress for around USD7.00 and was at first hesitant that the order might never arrive, or that they would send me the wrong part. It took about two and a half weeks for standard (free) shipping and I couldn't be any happier that they did send me the actual product that was advertised.

MacOS is known to be very particular with which chipsets they are compatible with. If you'd prefer not to get this wifi module, you can get a list of supported chipsets from [osxlatitude](http://forum.osxlatitude.com/index.php?/topic/2120-inventory-of-supported-and-unsupported-wireless-cards/).
