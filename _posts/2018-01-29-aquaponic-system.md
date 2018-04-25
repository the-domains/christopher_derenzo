---
publisher: {}
datePublished: '2018-04-25T00:28:44.392Z'
dateModified: '2018-04-25T00:28:43.093Z'
description: >-
  This project stemmed from the successes of previous projects to create a 99%
  autonomous eco system for fish and plants with the help of an Arduino for
  environmental controls.
via: {}
sourcePath: _posts/2018-01-29-aquaponic-system.md
title: Aquaponic System (personal)(2018)
hasPage: true
inFeed: true
author: []
starred: true
datePublishedOriginal: '2018-01-29T19:05:30.997Z'
url: aquaponic-system-personal2018/index.html
_type: Article

---
# Aquaponic System (personal)(2018)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/a03ee586-8d9f-453c-9943-c44543785e77.jpg)

This project stemmed from the successes of previous projects to create a 99% autonomous eco system for fish and plants with the help of an Arduino for environmental controls.

---

![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/a33667bf-a98a-4a62-97b9-9b328708ba2c.jpg)

The materials used for this project were mostly spare and used parts from past projects. From basic construction and thoughtful design to intricate wiring and calculated plumbing, power and air flow helped complete this fully automated aquaponic system.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/6a0fd0748d44e4ff2a1cb0437d73dbb7cf1f07e6.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/9c8ed1569273efa13c39117f9698462f92243efe.jpg)

The beginning started with a 150 gallon Aquarium and some lights just sitting around in the garage.

Then the purchase of a 3' x 5' x 6.5' tent w/ extras ($100) and a LED light fixture ($150)...

I anticipated building out a small framed in room, however the cost of the tent with extras was more affordable and sufficient for the space I had available!
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/b9d80c1ebf892caa243a17285faf001b23b7b695.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/d9df0a8478f1223fb51261a0d1dffb585d7bf208.jpg)

After putting the aquarium together and powering the tent with everything needed to control the environment inside, I then started to automate the system with spare supplies sitting around.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/4ab587205aacc890c9e06141c292ce395b0f0f72.jpg)

Snip the four tabs on the common side to power 8 outlets instead of 4\.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/19dfd3c285d9cd9ff5e0cccf37147440bf6d657e.jpg)

8 relays to control the outlets.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/a94cb0d79ba7b883809fe9c52ae69bd90fc6d3f9.jpg)

Relays, modified outlets and 2 surge protectors... Boxes to house the components and connectors to clean up and protect all the connections:
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/615c0d18a13ca670c04f73bc296e8765daadaace.jpg)

There is nothing like standing on a ladder to solder connections!
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/28e561861c37e7c4a988a22c48d43ad83ee5f3c0.jpg)

Transistors to control the relays.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/1946f3b3-9f15-4b32-98cc-01f99e37a44b.jpg)

From bread board to Thru-hole soldering the back of the circuit board, I work with what I currently have.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/a237778f-3f72-4e2f-aa02-b07cbe1d0f23.jpg)

Place it in a box with a 2.5mm power and a 50 pin d-sub connector so I can close the door and it can be easily serviced in the future.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/82f8904fd340682d83e4d90d69b04fd7d4d5db28.jpg)

Add two AC dimmers to the power box for digital control of 6" centrifugal fans for intake and exhaust. Notice this is where the current sensor is also mounted on the bottom of the box.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/d0c8ba73fb5a475e591680af2b791f6eec8da2d7.jpg)

---

After the power, controller and sensors are installed it's time to program:

Let's manually control it with a web browser and pull some information about the sensors too!

Most of my 4 week buildout was spent programming... With a multitude of global variables and algorithms the code underwent 57 revisions before it was complete and ready to run the machine without any user interaction! Each new revision incorporated a new feature or replaced an early idea with a better one, for example: Three temperature sensors all displaying measurements a couple of degrees off from each-other while being located in close proximity... Well, why not sum the data and react based on the average!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/f8037720-46c4-49fa-a418-ea9d96fa4945.png)

Another troubleshooting instance was when one of the sensors fell to the bottom of the tent after not securing it properly the night before. I'm sure you can guess that I found it in a small puddle of water the next morning which was just enough to cause a short and lead me to install a different sensor. (Yay... more code!) In the end I am sitting quasi-happy with 64% of dynamic memory used up and just over 3500 lines of code to operate this living/ breathing machine! There is ALWAYS room for improvement... TBC!

To wrap up the programming I wanted to see the sensor data outside of my serial connection to the Arduino... a small 20x4 LCD did the job just fine!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/b3d90dc7-7671-4016-beaf-79e6db341822.jpg)

Showing power consumption...
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/4ba9cccaa6fda1a119c33b4be8a958f23bfce7f2.jpg)

Water temp and garage temp...
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/e4b91ade08c9bb04a305a9f438586c421a71450a.jpg)

Outside temperature to control intake fan...
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/35f782ab-719c-4f9e-9bef-e0e8ef02a249.jpg)

and one of the sensors inside the tent to affect the exhaust fan...

It's also a good idea to be able to see the state of the 8 relays remotely and control them in the case of typical service so let's throw in a web controller!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/cbc7de93-e3e6-418b-aece-49e74799a513.jpg)

---

![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/268d731b588afec1217e60af59eb85156d2059ac.jpg)

Then it's time to take a break from programming to handle the last bit of construction beginning with the sump/ reservoir/ planter box. This is where the water will drain from the aquarium into the substrate (clay pebbles) and nitrites (good bacteria) will collect to break down the ammonia (fish waste) into nitrates (plant food).
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/74a1f8b207d9d478a9250ad8097cc573743784dd.jpg)

Notice the decline in the bottom for the water to flow down in the sump to reduce the amount of water needed inside of the tent. This will help keep humidity to a minimum and reduce the amount of extra water needed for the system.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/57d08f9596137b3638a1ddf0ed69d3d7768a16b2.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/56782f70279974c9bcbfb027bedc0830326c1dc5.jpg)

I found some unused plexi sitting around and cut it to size to fit between the substrate and plastic inside the box.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/2f6602f7710458bfebff2f25dc82f5a586086c40.jpg)

Finish the outside with a torch to bring out the features of the wood and coat it with boiled lynseed oil to reduce moisture damage.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/b73f4f992204d8d19de00303d1a66e6343203fd0.jpg)

It's time to machine about 700 individual holes in this acrylic base. Start off with a drill press...
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/83e1948464927abae8fd41ebeacd4954ac69438c.jpg)

...and finish with the hand drill.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/4e11a04348185db28b0dbe5b854389871042de09.jpg)

Sand the edges and seat it to ensure no damage to the 6mm plastic that will be fitted inside of the box.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/afc85dd3be95ff2db20300beed51c70680d6e7e1.jpg)

Coming together nicely.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/021e216ee5dc690ef1fd064ff61cc9311d999e50.jpg)

Let's put it in the tent to add the Hydroton and start the plumbing.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/8170d34333ddd5e73be6cb60d86faab1724d63c4.jpg)
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/b839f1638bca99edae373997403e7fa2baa61587.jpg)

150L of expanded clay pebbles fill this 39"x 19" x 14" space perfectly!
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/d257ce7155325e2984abea83e6d4057e5bdf5761.jpg)

Plumbing with 1" PVC for both the send and return.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/c2643fd5-49e4-4dad-a53c-96c0c55731ad.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/c195e719-a556-4ffa-8641-c6288cb14494.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/794dcc8b-3d47-46ed-9e4a-aacfc401f1ee.jpg)

(4) 1/2" outlets pre drilled water dispensers on the the gravity fed return from the tank.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/79d0bc2145b78778ceec317821dbe5c248d480d4.jpg)

Oxygen... Check!
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/05a102bb-cc76-4a55-9b7c-d041bb8480cb.jpg)

Water inlets to the tank are also 1/2" and provide clean water from the sump pump which is pushing uphill about 6' in height over 20' of distance which i show below is a little less than 79GPH \[insert frown face\]...

To start with some plumbing calculations, I need to turn about twice the capacity of the tank every hour, thats about 300GPH and the current 800GPH sump pump produces 13.33GPM (we will need this later) at the pump. Now we factor distance, and friction into the equation to see what we receive at the top of the aquarium return:

Total **Dynamic Head** is equal to **Static Head** (or "vertical lift") + **Friction Head**

**6'** of vertical lift from bottom of pump to top of tank

**Friction Head** is "the equivalent length of pipe" + the actual length of pipe times the "friction loss" and divided by 100\. eLength + aLength x friction ÷ 100

eLength =

20' total pipe distance (20' of head pressure)

8- 90˚ elbows (plus 8' of head pressure)

4- 45˚ elbows (plus 2' of head pressure)

30' is the **equivalent length** of pipe + 20' of actual length of pipe...

and **friction loss** is for 1" pipe at 13.33GPM which I used 13GPH for an estimate of 10.25 based on Table 2 of page 3 of the following article:

http://abe-research.illinois.edu/pubs/factsheets/SumpPumps.pdf

**Friction Head** = 30 + 20 x 10.25 ÷ 100 which is **5.125**

**Dynamic head** = 5.125 + 6 = 11.125 or 11 Feet

and this site identifies 10.8 feet of head loss with 4.7 psi at the top of the tank (not a lot of pressure there)

https://pentairaes.com/pump-calculator

So if this pump is rated to max out at 11 feet (manufacturer specifications), it is time to invest in a stronger pump! According to the pump manufacturer a 1200GPH pump will provide just over 500GPH at 11 feet of head height which is more than sufficient for this application and will provide additional control over the flow rate.

This would explain why my bell siphon is gurgling (breathing) every twelve seconds.

What a fascinating project to have sitting next to your workspace. It is relaxing listening to it breathe and what a joy to watch as it becomes a place for future fish and plants to thrive!

Next stop some fingerling tilapia!

---

While waiting for the tilapia I have found that my power usage, according to the current sensor and my latests power bill, puts me in Tier 3 or the "High Usage" bracket and this does not even take into consideration the use of an air conditioner and dehumidifier running 24 hours a day. That will require another 10A of power which more than doubles the average power consumption throughout the day. I have found a another way to control an environment that will produce great plant vegetation. An infrared temperature sensor will help me identify the temperature of the plant leaves to help me establish a new control of the environment with only an intake and exhaust fan and a low power sonic vaporizer for humidity.

In nature, plants sweat just like humans do to cool off and during this process they will absorb more water and nutrients through their roots. By forcing the plants to uptake nutrients you can relocate the Nitrates from the fish waste and into the plant thereby increasing plant growth. (Yay!)

So to create a comfortable environment for plant to thrive I will need the temp of the plant leaves, the ambient temp and humidity of the environment and I will use a calculation for vapor pressure deficit (VPD) to control the rate and frequency of the fans and humidifier instead of controlling the tent with power hungry appliances.

What is VPD? First, water vapor that is in the air exerts a certain pressure on the plant leaves to allow for the pores to open and close. Second the saturated vapor pressure is how much moisture the air can hold at a given temperature or the point of equilibrium where the number of water molecules evaporating are the same as the ones that are condensing. So the deficit is the difference between vapor pressure and the point of saturation in kPa. 

Deficit = (Saturation Vapor Pressure) - (Actual Vapor Pressure)

SVP (kPa) = 0.6108 \* exp(17.27 \* T / (T + 237.3))

AVP (kPa) = RH / 100 \* SVP

_vpd = \[0.6108\*exp((17.27\*plantTempC)/(plantTempC+237.3))\] - \[0.6108\*exp((17.27\*plantAmbientTempC)/(plantAmbientTempC+237.3))\*tentHumd/100\]_

This function measures the plant temp, ambient temp and relative humidity. Each type of plant reacts differently to various settings so I will use this opportunity to investigate this new variable and see what comes of controlling the environment by VPD.

---

![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/be1cc002a812686086ae0eac33387b08183c5f4d.jpg)

Now the fish have arrived and I have to prepare the tank for farm raising fish (tilapia), I need to test and raise/ lower the PH and total dissolved solids (TDS) to the recommended levels for similar aquaponic systems proven to be successful. PH for tilapia is best at 8.0 and for plants approximately 6.5 so this means I will set it somewhere between 7.2 and 7.4
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/4056f61b70eac7f2d4cf040a7303d4d089b74a01.jpg)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/713296e9-85ef-415f-8e82-50cd6a75233f.jpg)

The water coming from the city of LA is exceptionally high in dissolved solids so it's time to consider some other filters for the fresh water going into the system.

---

Here is some data displaying VPD and Power in relation to other sensors:
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/5dd9dab9-13a4-453b-bff8-e490ff9d63cf.png)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/88c7cc8c-2e16-48dd-b302-96106bd0d35f.png)
![](https://imgflo.herokuapp.com/graph/2b2431f8e7ba7b0/8c75377c86cbec84f7d517e1333f46f3/croprotate.png?cropheight=680&cropwidth=1018&degrees=0&input=https%3A%2F%2Fthe-grid-user-content.s3-us-west-2.amazonaws.com%2Fe3b9adfb-52d2-41d4-965a-f3765cd75695.png&x=0&y=1)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/04bdd93f-e890-4e4e-9eb8-8c3e483f26ec.png)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/147b325e-d7af-4404-b2dc-b0368605cdce.png)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/a907e7a2-9e9d-404b-881b-3cb4391b7e12.png)
![](https://imgflo.herokuapp.com/graph/2b2431f8e7ba7b0/a6fe47b8eee2e6d79d7f71c052ab971e/croprotate.png?cropheight=680&cropwidth=1018&degrees=0&input=https%3A%2F%2Fthe-grid-user-content.s3-us-west-2.amazonaws.com%2F25ecb24b-7010-4408-859f-44747d76ce85.png&x=0&y=1)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/b1306dd3-ea16-462b-9ec7-c9066125f7ab.pdf)