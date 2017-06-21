---
layout: post
title: IoT Hackathon on Smart Environments @HHZ_BB
subtitle: Smart Environments for Teaching and Learning
share-img: "http://cdeck3r.github.io/img/blog/IoT_Hackathon_SS17.png"
bigimg:
  - "/img/blog/IoT_Hackathon_SS17_bigimg_0.png" : "IoT Hacking (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_1.png" : "Testing Dash Buttons (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_2.png" : "Presenting Stay Focussed Project (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_3.png" : "Testing IoT Devices (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_4.png" : "Presenting Smart Doorbell Project (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_5.png" : "Discussing IoT Development (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_6.png" : "Presenting various Dash Button Use Cases (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_7.png" : "Concentrating on IoT Hacking (2017)"
  - "/img/blog/IoT_Hackathon_SS17_bigimg_8.png" : "Color coding of FarbenFroh Project (2017)"
---


This term's IoT hackathon in the masters programme on [Services Computing](http://www.hhz.de/master/services-computing/) was about Smart Environments, where IoT services support various teaching and learning activities.

![IoT Hackathon SS 2017](/img/blog/IoT_Hackathon_SS17_title.png)

## Background & Motivation 

Teaching and learning at the [HHZ](http://www.hhz.de) is characterized by block courses enabling part-time Master's studies for working professionals. Lectures last the entire day. There are lots of hands-on exercises, which help to achieve a good balance between focused learning and practical activities. However, it is a challenge to organize all activities taking the current situation during a lecture into account. 

The Internet of Things (IoT) constantly accessible and interwoven into our daily routines may support activities for a situation-aware and student-tailored teaching and learning. 

Ultimate goal of this hackathon is to explore IoT services which are *permanently* installed and used by students and lectures at the HHZ. Both lecturers and students shall benefit from these services.

## Sensor-instrumented Room

The hackathon utilized an sensor intrumented environment installed in our lecture room. The Arduino based wireless sensor network was evaluated in the [last term's hackathon](/2017-01-18-SCM-IoTHackathon). The following sensors were deployed multiple times at various places in the room.

* Movement
* Temperature
* Humidity
* CO2

A Raspberry Pi served as central data collector and runs [Home-Assistant.io](https://home-assistant.io/) providing a dashboard and REST interface to all sensors. 

## Projects for Building Smart Environments

Students were required to *transform the sensor instrumented room into a smart environment*.
They proposed various additional devices, such as Amazon's Dash Buttons, smartphones, and Philips Hue light system.

All projects are publicly available. Checkt out the following links:

* [StayFocussed](https://github.com/jules185/IoT_Hackathon/wiki) - A service enabling improved concentration during lectures providing recommendations.
* [FarbenFroh](https://git.io/vHQCx) - Sense, evaluate and display, in particular using peripheral perception, the current quality of lecturing environment
* [Dashbutton](https://github.com/cin9/hhz_hackathon_dashbuttons/wiki) - Three IoT use cases of what you can do with an Amazon DashButton.
* [Emergency Button](https://github.com/91kodi1bvg/Emergency-DashButton/wiki) - Call for help and confirm.
* [Smart Doorbell](https://github.com/chiefblub/IoTHackathon/wiki) - How to enter the HHZ for learning and project activities outside the opening hours.
