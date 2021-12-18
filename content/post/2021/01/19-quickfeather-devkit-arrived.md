---
title: "The QuickFeather Dev Kit has Arrived "
date: 2021-01-19
tags: ["hack", "play", "quickfeather"]
image: https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1611055740/hackworkplay/IMG_20210119_140327.jpg
---
I joined a hackster.io challenge called [Challenge Climate Change](https://www.hackster.io/contests/quickfeather) and won some free hardware.

<!--more-->

![photo of the kit](https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1611055740/hackworkplay/IMG_20210119_140327.jpg)
*The box, a CP2102 and the QuickFeather*

Here's a link to the application I've made: https://www.hackster.io/contests/quickfeather/hardware_applications/13290 and reproduced here for posterity:

# Citizen Science: Distributed Air Quality Monitor and Prediction

## What problem are you going to solve?

Most of the air quality monitors in my country are located outside of residential areas, and so the reports are not that accurate since they would only be based on certain hotspots.

## What are you going to build to solve this problem? How is it different from existing solutions? Why is it useful?

I'm building the initial prototype to try and see the BOM, then find out how to reduce the cost so it can easily be manufactured and distributed to anyone. The difference from other commercial products is that the whole thing would be open-source and open-hardware such that anyone else can build the product themselves if they are inclined to.

When deployed, the sensors would optionally be connecting to a central hub that would gather data and visualize the information in graphs and maps.

The individual sensors can also optionally display certain predictive actions (like closing windows) whenever conditions are met (for example, when the air quality is predicted to become worse because of statistical history)

## How does your solution work? What are the main features? Please specify how you will use the QuickFeather and SensiML AI Software Bundle in your solution.

The QuickFeather will be the "brains" of the operation, together with a honeywell PM2.5 and PM1.0 particulate matter sensor, and a CCS811 + HDC1080 for temperature and eCO2/TVOC sensing (I already made a prototype, albeit more bulky and more expensive, here: https://www.element14.com/community/groups/roadtest/blog/2020/11/13/road-testing-the-pan1780-evaluation-kit-part-5-air-quality-dashboard-via-web-bluetooth)

The difference is that I want to setup the network portion via nodered and advertisements, which would then send the data to a server to collate and hopefully analyze possible hotspots of pollution.

## List the hardware and software you will use to build this.

* HPMA115S0-XXX Gas Detection Sensor PM2.5 PM1.0
* AMS CCS811 eCO2 TVOC sensor
* TI HDC1080 Temperature sensor
* Raspberry Pi 4 (optional, can be replaced with a laptop)
* Node Red
* Postgres (optional, can be replaced with mysql/mariadb)
* Javascript (for visualization)

## Tell us about yourself. What do you spend most of your time doing? What skills or experience do you have that will enable you to be successful in building this project?

I'm a software developer with an electronics hobby. I recently did a review of a bluetooth low energy eval board from panasonic and various other blog posts over at hackaday:

* https://www.element14.com/community/roadTestReviews/3491/l/panasonic-pan-1780-bluetooth-le-eval-kit-review
* https://hackaday.io/projects/hacker/895883

