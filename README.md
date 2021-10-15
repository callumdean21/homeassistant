

# 							Smart Home Configuration 

### 										Home Assistant Guide for my Smart Home



------

[TOC]

#### Home Assistant Hardware

|                     Raspberry Pi 4 B 8GB                     |     Dual Fan Aluminium Heatsink Case for Raspberry Pi 4      | Sandisk Extreme microSDXC 128GB                              | Raspberry Pi 4 USB-C 5.1V 15.3W PSU                          |
| :----------------------------------------------------------: | :----------------------------------------------------------: | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](https://core-electronics.com.au/media/catalog/product/cache/1/image/650x650/fe1bcd18654db18f328c2faaaf3c690a/p/i/pi-4_1_1_1.jpg) | ![](https://core-electronics.com.au/media/catalog/product/cache/1/image/650x650/fe1bcd18654db18f328c2faaaf3c690a/d/u/dual-fan-aluminium-heatsink-case-for-raspberry-pi-4-black1-2.jpg) | <img src="https://shop.westerndigital.com/content/dam/store/en-us/assets/products/memory-cards/extreme-uhs-i-microsd/extreme-uhs-i-microsd-128gb.png" style="zoom:25%;" /> | ![](https://core-electronics.com.au/media/catalog/product/cache/1/image/650x650/fe1bcd18654db18f328c2faaaf3c690a/a/u/au_psu_black.jpg) |

This hardware isn't anything amazing, but for my current needs it is more than satisfactory, and should be future proof enough to see me well into the next few years of automation.

------

#### Home Assistant Software

![](data:image/png;base64,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)



Obviously I am running the latest version of Home Assistant (ver 2021.3.4 at time of writing) on the hardware listed above. For my current needs this is more than enough to run my instance of Home Assistant.



On top of this vanilla install of Home Assistant I am also running a few other applications, as listed below:



<img src="http://fabacademy.org/2019/labs/napoli/students/ntngrillo/assignments/img/w16/node-red-logo.png" style="zoom:25%;"  />

###### Node-RED

Currently I am only using Node-RED to run a script to integrate my Smart Robot Vacuum (Roborock S6 MaxV), as there is no native integration with Home Assistant for newer models of the Roborock vacuums. This was achieved (after many headaches) by using a 'token extractor' developed by Piotr Machowski (https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor). This token then can then be inputted into the Xiaomi Roborock connectivity nodes (https://flows.nodered.org/node/node-red-contrib-miio-roborock) in order for me to issue simple commands to my vacuum cleaner from inside of Home Assistant.



<img src="https://www.zigbee2mqtt.io/images/logo.png" style="zoom:50%;" />

###### Zigbee2MQTT

In order to circumvent the nightmare that is proprietary Zigbee hubs, and still capitalise on the many benefits of Zigbee, I am currently running Zigbee2MQTT in tandem with Mosquitto to handle the MQTT side of things. In order to 'talk' to my Zigbee devices I am using a CC2531 purchased from eBay (https://www.ebay.com.au/itm/224344010798?chn=ps&mkevt=1&mkcid=28). This allows me to 'sniff' Zigbee data and convert each 'sensor' to a topic in MQTT which means I can then detect posts to these topics based upon a change in state of the sensor and detect this as an update in Home Assistant, or run this process in reverse, and publish a message to one of the sensor's topics in order to facilitate a state change.



<img src="https://obrienlabs.net/images/content/mosquitto_logo.png" style="zoom:25%;" />

###### Mosquitto

As I mentioned earlier, Mosquitto is used to handle all of MQTT back and forth from the Zigbee devices. Nothing special here, just a basic installation of Mosquitto that is subscribed to the topics that my sensors are posting to.



<img src="https://grafana.com/static/img/logos/grafana_logo_swirl-events.svg" style="zoom:50%;" />

###### Grafana

This is a fairly new addition to the arsenal, and I am beginning to use Grafana map and view data over time, in an easy to read format. Currently I am tracking power usage from a few devices, and graphing this to track consumption. Once again, nothing revolutionary



<img src="https://www.nabucasa.com/img/default-social.png" style="zoom:33%;" />

###### Nabu Casa

I'm running Nabu Casa for 2 main reasons: 1) To be able to access Home Assistant via the Android App, 2) in order to cast Home Assistant to the 2 Google Home Hub's that I use as in home interfaces. 

------

#### Network

Considering I create, and maintain networks for a day job, you'd think my home network would be something a bit more interesting, however this setup has filled my needs (in its various iterations) for several years now. Below is a map of my network, and its function.

<img src="C:\Users\Callum\OneDrive - The Yiros Shop\Documents\Network Topolgy.jpg" alt="Network Topolgy" style="zoom: 150%;" />

Currently my Internet is powered by the Huawei B818 modem, to connect to 4G, however this is in bridge mode due to having incredibly limited functionality out of the box. 

My TP-Link Archer C2 is used to handle all of the actual networking, as like previously stated this is not a strong suit of the B818. I am running 2 separate Wifi channels, one on 2.4Ghz, and the other on 5Ghz. Obviously I prioritise the 5Ghz signal for devices that are close enough (and equipped) to receive it, however the 2.4Ghz is there for those older devices, and devices that are just that little bit too far from my router to pick up the 5Ghz signal.  The Archer also handles IP allocation, and all of my sensors and smart devices are assigned a Static IP outside of the DHCP reservation to remove any possibility for things to get confused with their IP addresses (this happens all too frequently if the IP addresses are assigned dynamically). 

1. The Raspberry Pi 4 B, is running off of BalenaOS, and is used as a Wifi Repeater, as my partner's office seems to be a black-hole for Wifi signals. I have been using Balena Etcher as my go-to SD Card Imager for a while now, and one day while etching 1 of the hundreds of SD Cards I have to write for work I noticed that Balena offered a Wifi Repeater tutorial (https://www.balena.io/blog/turn-a-raspberry-pi-into-a-wi-fi-access-point-or-repeater/). This started as an excuse to tinker with Balena, and the possibilities that batch-editing, and cloud-access to Raspberry Pi's opened up for me in my work life, and ended up being a damn good wifi repeater.

I am looking at upgrading this network in the near future and replacing it with some Unifi gear from Ubiquiti. Below is a more detailed look at my proposed network map (if I can ever justify the $$$)

![Ubitquit Topology](C:\Users\Callum\OneDrive - The Yiros Shop\Documents\Ubitquit Topology.jpg)

------

#### Voice Control and TTS

In Australia, for the longest time, there was only 1 choice when it came to Voice Control; Google. When Amazon first released their products they were not available in Australia, and up until very recently although available they weren't supported. This meant that as an early adopter of this technology I was only left with one option. At the time I had just moved myself and my partner across to Google Pixel's from our iPhones, and i felt that the Google Home was the natural next step.



Currently in my home I have:

- 1 Google Home
- 3 Google Home Mini
- 2 Google Home Hub
- 2 Google Pixel 4XL

This is somewhat overkill, but I seem to be a lamp, that everyone Google Home's gravitate towards like moths, when the original owner gets over the novelty of "Hey Google! What sound does a cow make?"

###### Voice Control:

Light Control - LED Strips, Wall Switches and Bulbs
Climate Control - Control our 2 Airconditioners
Media Control - Turn on/off Media Devices, play Media

###### TTS

Although currently I dont really use any TTS (except for a talking clock script created in Node-RED by my father), it is something that I have toyed with the idea of for a while now. Half of me thinks it would be great to get TTS notifications about certain events, while the other half thinks about how quickly it would get turned off after the novelty wears off.

------

#### Sensors

I originally began using Home Assistant because I had too many sensors, all with proprietary apps to track, and while it all made sense to me, my partner could not make head nor toe of it and thus would not use the system correctly.



<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Xiaomi_logo.svg/480px-Xiaomi_logo.svg.png" style="zoom: 25%;" />

###### Xiaomi

I have a Xiami Aqara Door sensor, to detect when the front door is opened/closed and this in tandem with my phone's GPS then triggers Automations such as vacuuming the house, or turning on the lights. 



<img src="https://upload.wikimedia.org/wikipedia/en/a/a1/Philips_hue_logo.png" style="zoom:33%;" />

###### Philips Hue

Philips Hue has always been the 'gold standard' in terms of Home Automation in my eyes, however having to buy a hub was big barrier to entry. This was removed with the advent of Zigbee2MQTT, and by god i'm glad it was.  I currently have 2 Philips combination Lux/Temp/Motion sensors positioned near both of my air conditioners in order to detect the difference in outside/inside temp, and turn on climate control until they are at equilibrum. The Lux sensors are also a good way to turn lights on/off without having to rely on Sunset/Sunrise times.

------

#### Lighting

For my lighting, once again it comes down to what was cheap/available at the time of purchase.



<img src="https://pbs.twimg.com/profile_images/1082466578489200641/xCt9mjmL.jpg" style="zoom:25%;" />

###### Yeelight (Xiaomi)

These were the first lights I ever bought, and they have always been some of my favourites. With a bit of work you can even put them into a local mode that doesn't require requests to leave your local network (very handy when the internet goes down). I currently have 3 Yeelight RGB Bulbs, and I use them in my lounge room as they have a good white gamut, as well as bright vivid colours that are great for Multimedia.

<img src="https://upload.wikimedia.org/wikipedia/en/a/a1/Philips_hue_logo.png" style="zoom:33%;" />

###### Philips Hue

These are a recent addition, and I only have 1 as I received it as part of a bundle deal. It works very well, and also has the added bonus that it acts as a Zigbee extender



<img src="https://www.logo.wine/a/logo/IKEA/IKEA-Logo.wine.svg" style="zoom: 25%;" />

###### IKEA Tradfri

These bulbs were purchased for 2 reasons: Affordability, and ability to extend my Zigbee network. They serve their purpose and I dont really have any complaints, except for the fact that they aren't tuneable, and are warm white (not a fan in tropical QLD).

------

#### Miscellaneous

This is the section for all the devices I couldn't fit anywhere else.

<img src="https://res-4.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco/lc0ax9y1razb1l9e9k0j" style="zoom:67%;" />

###### Roborock S6 MaxV

As the owner of a Japanese Spitz in a sub-tropical climate, I'm no stranger to dog-hair (or *floof* as my partner likes to call it). After countless hours of watching reviews, comparing features and price the Roborock S6 MaxV seemed to come out on top, and also seemed to have a pretty easy workaround for controlling it via Home Assistant. I had this vaccum for a little over 9 months, and I must say it has been one of the best things I have ever purchased. vacuuming, mopping, sweeping it does it all!

------

