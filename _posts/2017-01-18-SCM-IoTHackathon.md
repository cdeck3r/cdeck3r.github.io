---
layout: post
title: IoT Living Lab for Teaching @HHZ_BB
share-img: "http://cdeck3r.github.io/img/blog/IoT_Hackathon_WS16.png"
bigimg:
  - "/img/blog/IoT_Hackathon_WS16_bigimg_1.png" : "IoT Hacking (2017)"
  - "/img/blog/IoT_Hackathon_WS16_bigimg_2.png" : "Internet enabled push button (2017)"
  - "/img/blog/IoT_Hackathon_WS16_bigimg_3.png" : "Sensor instrumented room presentation (2017)"
  - "/img/blog/IoT_Hackathon_WS16_bigimg_4.png" : "Real-world Like button (2017)"
  - "/img/blog/IoT_Hackathon_WS16_bigimg_5.png" : "IoT software development (2017)"  
---


Today, the students gave their final presentation of their hackathon projects. 
It is a part of my IoT lecture in the [masters programme "Services Computing" (SCM)](http://www.hhz.de/master/services-computing/) at the HHZ. 
The hackathon's topic was to support the teaching and learning as part of a permanent 
[Living Lab](https://en.wikipedia.org/wiki/Living_lab) implemented in our lecture rooms. 

![IoT Hackathon WS 2016](/img/blog/IoT_Hackathon_WS16_title.png)

## Approach

Each of two groups has designed and implemented an application use case within two days. 
Starting with a coarse concept, students used their know-how from the IoT lecture and other SCM lectures to explore
and design appropriate IoT services, explain the the value proposition and architecturing an [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product). 
As a result, the MVP was implemented and demonstrated.

## Projects

### Beacons for the Sensor Instrumented Room

Sensor instrumented environments enable and support various application use cases. 
A common problem is to discover the access entry point of provided services. The internet knows the DNS, 
but in IoT environments users constantly changes their network affiliation making it hard to find and access changing 
network-based services. 
Bluetooth beacons are a nearfield communication technology supporting location-based service discovery in IoT environments. 

The group implemented a room environmental monitoring system using Arduino based wireless sensors. 
Data is collected on Raspberry Pi server. A bluetooth beacon at the room's door entrance pushes the URL of the 
server to mobile phones of nearby lecture participants. The system is used to inform about the room's micro-climate
and helps to create an comforatable environment for teaching and learning.

Check out the [project's repo](https://github.com/tim8890/hhz-hackathon-team-beacon/wiki/Wiki)

### Concept of Real-World Likes

We all know the "like" button in social networks such as facebook, twitter and others. 
Currently, there are already electronic systems deployed implementing a real-world "like" button,
see [happy-or-not.com](https://www.happy-or-not.com/de/messung/) for example.

This project transfers the concept of "likes" into the real world and explores what one can do beyond "like". 
A button seems limited in its functionality, but at the same time its usage is easy to understand. 
Rich applications are enabled by the context corresponding with the button. In the real world, 
the situation and the question-to-like determine this context. Both may easily change the meaning of pushing a button and
therefore generating very expressive "likes".

Using internet enabled push buttons, 
e.g. [Particle.io Button](https://www.particle.io/products/hardware/internet-button), students and 
lecturers at the HHZ can now utilize electronic support for various activities and communicate more than just "yes/no" or "like/dislike".

Check out the [project's repo](https://github.com/hhz-hackathon-2017/IotHackathon) for more details. 

## Further information

All projects are publicly available. Checkt out the following links:

* Beacons for the sensor instrumented room, https://github.com/tim8890/hhz-hackathon-team-beacon/wiki/Wiki
* Concept and Implementation of Real-World Likes, https://github.com/hhz-hackathon-2017/IotHackathon


