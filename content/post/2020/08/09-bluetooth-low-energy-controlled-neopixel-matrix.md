---
title: "Bluetooth Low Energy Controlled Neopixel Matrix"
date: 2020-08-08
tags: ["hack", "play", "neopixel", "ble", "nrf52832"]
image: https://res.cloudinary.com/psqd/image/upload/v1600853419/hackworkplay/7698761596956604215.jpg
---
I accidentally lifted some of the pads off of my Ebyte nrf52832 bare module and that means I won't be able to use it as a development and test board anymore.

<!--more-->

Get the nRF52832 module here: https://psqd.pw/ebyte-bare

That also does mean I can use it on a more permanent fixture, so that's what I did.

I've been looking to have my neopixel matrix more autonomous by connecting it with a wireless microcontroller and having that as a single unit. This ebyte module is perfect to integrate with the matrix, giving me the ability to control it remotely via Bluetooth Low Energy.

I've already installed Espruino on the module, so all I needed was some sticky tack and wires (and a 3v3 regulator I salvaged from another project that didn't quite go as planned).

![some chips attached to the back of a flexible pcb](https://res.cloudinary.com/psqd/image/upload/v1600853419/hackworkplay/7698761596956604215.jpg)*I added the button because Espruino supports DFU updates and you do that by holding BTN1 (which in this firmware was P14) during bootup.*

Here's the javascript program for the BLE control:

``` javascript
const neopixel = require("neopixel");

const rows = 8;
const cols = 8;
const bpp = 24;
const ledCount = 64;
const pin = 25;
const leds = Graphics.createArrayBuffer(
  rows,
  cols,
  bpp,
  {
    zigzag:true,
    color_order: 'gbr'
  }
);
leds.flip = () => { neopixel.write(pin, leds.buffer); };


const scale = (num) => num / 0xFF;

NRF.setTxPower(4);
NRF.setServices({
  "0x181C": {
    "0x2A3D": {
      value: [0,0,0,0,0],
      writable : true,
      description: "sets the value of a pixel: [r, g, b, x, y]",
      onWrite : function(e) {
        const data = new Uint8Array(e.data);
        leds.setColor(scale(data[0]), scale(data[1]), scale(data[2]));
        leds.setPixel(data[3], data[4]);
        leds.flip();
      }
    }
  }
}, { advertise: ['181C'] });


NRF.on('disconnect', function() {
  leds.clear(true);
  leds.flip();
});

E.on('init', function() {
  NRF.setConnectionInterval(7.5);
  console.log("Hello World!");
  leds.clear(true);
  leds.flip();
});
```
If you write a byte array of [r, g, b, x, y] to the 0x2A3D characteristic, that particular pixel in the matrix will light up. Disconnecting will clear the whole matrix.

![an led matrix](https://res.cloudinary.com/psqd/image/upload/v1600853416/hackworkplay/1260901596956821958.jpg)*The whole thing was done at the back, so all that really shows up in front is the power cable.*

-----

*this post also appears on https://hackaday.io/project/174219-oneoffs/log/181978-bluetooth-low-energy-controlled-neopixel-matrix*
