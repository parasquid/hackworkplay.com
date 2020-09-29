---
title: "ESP32 Cam Dev Board and Tools"
date: 2020-08-15
tags: ["hack", "play", "esp32", "wire wrap"]
image: https://res.cloudinary.com/psqd/image/upload/v1600853428/hackworkplay/7834841597488054290.jpg
---
The You tube algorithm decided to show me some ESP32 Cam videos and I remembered I had a couple in storage. So I thought, why not try it out again and refresh my experience with it?

So I brought out my perfbaord and wire wrapping tools and decided to create a more or less generic board for the module.

<!--more-->

![Dev board and some wire wrap tools](https://res.cloudinary.com/psqd/image/upload/v1600853428/hackworkplay/7834841597488054290.jpg)

That's really all there is to it. Double rows of female headers (to accommodate male dupont connectors), male headers on the inside for the semi-permanent wire wrapped connections, and male headers on the outside for female dupont connections.

There's also the serial 90-degree bent headers for connecting the USB-serial programmer (its pin order is that of the Arduino pro mini, but since this is a wire-wrapped jig, it's not that difficult to change the assignments if I ever want to assign a permanent USB-serial programmer for this dev board).

I also added a button that would pull GPIO0 to ground since that's required to bring the ESP32 Cam to bootloader mode (hold it down on startup to enter that mode).

Speaking of wire wrap tools, I have a counterfeit clone bought from a well-known chinese website, as well as the original one bought from digikey:

![Wire wrap tools, the original and a counterfeit](https://res.cloudinary.com/psqd/image/upload/v1600853425/hackworkplay/7687551597488329281.jpg)

They function mostly the same, but there are some subtle differences:

* the clone takes in a couple mm of the kynar coated wires when inserted while the original just stops the wire insulation right at the lip. The pvc insulation is too thick for either tool to ingest.

* the original has a much sharper insulation stripper (although this may be due to the fact that I use the clone more)

* the original has more heft and weight to it, and feels more "premium" (like steel vs aluminum)

* pvc coated wires wrapped with the original tend to overlap, while I generally have no issues with wrapping on the clone; I don't have any issues when wrapping with kynar coated wires on either of them

Also, while trying to find the ESP32 Cam I saw an old dev board I made for the ESP32 NodeMCU:

![Underside of some dev boards](https://res.cloudinary.com/psqd/image/upload/v1600853425/hackworkplay/7158731597488763932.jpg)*The left one is the dev board I just made, and the right one is the dev board I made a some time ago. Hard to imagine I soldered like this back in the day!*

-----

*this post also appears on https://hackaday.io/project/174219-oneoffs/log/182243-esp32-cam-dev-board*
