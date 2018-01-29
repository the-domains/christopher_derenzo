---
publisher: {}
datePublished: '2018-01-29T19:58:13.332Z'
dateModified: '2018-01-29T19:58:06.205Z'
via: {}
description: >-
  This project stemmed from the successes of previous projects to create a 99%
  autonomous eco system for fish and plants with the help of an Arduino for
  environmental controls.
title: Aquaponic System (2018)
sourcePath: _posts/2018-01-29-aquaponic-system.md
inFeed: true
author: []
starred: true
datePublishedOriginal: '2018-01-29T19:05:30.997Z'
_type: Blurb

---
# Aquaponic System (2018)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/a03ee586-8d9f-453c-9943-c44543785e77.jpg)

This project stemmed from the successes of previous projects to create a 99% autonomous eco system for fish and plants with the help of an Arduino for environmental controls.

The materials used for this project were mostly spare and used parts from past projects. From basic construction and thoughtful design to intricate wiring and calculated plumbing, power and air flow helped complete this fully automated aquaponic system.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/9c8ed1569273efa13c39117f9698462f92243efe.jpg)

The beginning started with a 150 gallon Aquarium and some lights just sitting around in the garage.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/b9d80c1ebf892caa243a17285faf001b23b7b695.jpg)

Then the purchase of a 3' x 5' x 6.5' tent w/ extras ($100) and a light fixture ($150)...

I anticipated building out a small framed in room, however the cost of the tent was more affordable and was sufficient for the space available!

After putting the aquarium together and powering the tent with everything needed to control the environment inside the tent I then started to automate the system with supplies sitting around in boxes.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/4ab587205aacc890c9e06141c292ce395b0f0f72.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/2b217e53-754d-40ab-99c1-0e55e6fa8f54.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/19dfd3c285d9cd9ff5e0cccf37147440bf6d657e.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/a94cb0d79ba7b883809fe9c52ae69bd90fc6d3f9.jpg)

Relays, modified outlets and surge protectors on two points... Boxes to house the components and connectors to clean up and protect all connections:

There is nothing like standing on a ladder to solder connections!
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/615c0d18a13ca670c04f73bc296e8765daadaace.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/899b3463-dc28-4d4e-a5bb-24016c79043e.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/0abb48ef-0867-4da6-acea-724562a2a4ba.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/aba0973f-1d74-4c67-932b-71a02a1496a1.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/0bd97d68-c55f-4a95-a681-dae55f664452.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/3e9f40a1-c45d-47e8-bbd5-60578e31f2af.jpg)

The next phase was the construction of a box to filter the water through substrate (expanded clay pebbles) and produce the natural bacteria for the plants. This is where the plants will live!

A little machining of some leftover acrylic glass:
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/17afd7a9-a9f6-4f19-83cb-d52bc0bbfa9d.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/8cb5bef2-e469-4cca-ae13-8610ffcdb069.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/b273544b-bcb8-4da1-bc4f-e3e10ee162ae.jpg)

Oh man, that's a lot of holes!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/03ef88e2-05bc-480d-8ce8-eed397421bfc.jpg)

A little plastic to hold the water...

and viola!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/76666716-7337-4226-86d4-6648e8b42d10.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/3314f32e-1e3e-41c0-92ca-5ec4ec7cc192.jpg)

To get the water we use 1" PVC with (4) 1/2" outlets on each end to reduce pressure and ensure equal disbursement of water
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/923ce3ba-b86c-40f7-b1df-7e075f043f1c.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/d27225b4-f4bb-4bb1-857b-aeaa0c1bf5de.jpg)

As it all came together the programming completed everything with a complicated scheduler and alarm that required communication with an NTP server to sync time with the Arduino. ![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/b602c600-6393-4191-a599-9b6f659e1eda.jpg)

To a wide assortment of variables and "if" statements polling sensors to operate according to specific environmental needs.

The code is the part that took the longest time to procure based on testing and re-coding and testing some more until finally it turns lights, fans, air-conditioners, humidifiers, dehumidifiers and pumps off and on at various times throughout a day!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/e0634173-e475-4e98-a8bd-f71c4bf223fe.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/06857313-0eac-426d-9d2c-383313e934cc.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/82d4ee28-77d8-48d5-b53e-7b9d4a1d0480.jpg)

After programming, it became necessary to see the status of the sensors to calibrate and verify correct operation of the components, hence the LCD display programmed to cycle through 5 different temp/ humidity sensors, power consumption, and date and time! Three of the sensors are located inside the tent calculating an avaerage to produce as close to perfect reading of temp and humidity to control the fans, AC, humidifier and dehumidifier... one more sensor is located inside of the garage for ambient temp and another is located outside to determine if it will pull air from outside! Oh yeah, one more temp sensor for the aquarium to identify the temp of the water... phew!

What a joy it is to to have the sights and sound of a tiny eco system with light, water and wind, breathing life through automation, just sitting right next to your workspace!