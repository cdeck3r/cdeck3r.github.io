---
layout: page
title: Smart Environments
subtitle: Intro / DDL / Research
share-img: "http://cdeck3r.com/img/blog/IoT_Hackathon_SS17.png"
---

**tl;dr - What is a Smart Environment?**

*video, tbd*

## Intro and Types of Smart Environments

A smart environment is a sensor and actuator instrumented room or space. Embedded networked computer systems make the room perceive physical state and activties within. In a smart environment physical routines and information processes may seamlessly interact with each other.

At the HHZ, we have implemented a smart environment to support [Data Driven Lectures (DDL)](/teaching/ddl). 
The installation runs 24/7 and supports students as well as lectures in learning and teaching activities. 

Bascially, we distinguish between three stages of extension for smart environments.

| Type | Description | 
| ------ | ------- |
| Remote Control | User control devices via apps; becomes more difficult to operate as the number of networked devices rise. Examples: weather station, alarm switches  |
| Reactive Environment | Networked appliances enable automation of routines; users may create automation rules. Examples: Home automation using [IFTTT](https://ifttt.com/) |
| Adaptive Environment | Autonomous learning of daily routine and its automation support; computers become invisible, i.e. no explicit UI, environment acts according to users' needs. Examples: Home automation using [NEST](https://nest.com/thermostat/meet-nest-thermostat/)  |

## Smart Environment for DDL

[Data Driven Lectures (DDL)](/teaching/ddl) aim at a continuous progress and quality monitoring of my lecturing activities
through the use internet technology. A classroom embedding various Internet-of-Things (IoT) technologies connects directly lecturing and learning activities. The room perceives the current situation of all attending students and enables immediate feedback and control on breaks, progress and pace of a lecture. As a result, it virtually appears that the environment reacts in an intelligent way, i.e. supporting the lecture. 

<iframe src="//www.slideshare.net/slideshow/embed_code/key/CoIdyMvD4fDRtG" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/ChristianDecker4/smart-environment-for-ddl" title="Smart Environment for DDL" target="_blank">Smart Environment for DDL</a> </strong> from <strong><a href="https://www.slideshare.net/ChristianDecker4" target="_blank">Christian Decker</a></strong> </div>

## Hardware and Software

* Controller: Raspberry Pi 3 running Home-Assistant (0.35.3) on Raspbian Jessie Lite (Kernel 4.4)
* Gateway and sensors platform: Arduino Nano (xcsource clone)
* Radio module: NRF24L01+
* Sensors: 
    * Temperature/Humidity sensor: DHT11
    * CO2 sensor: MQ135

## Research and Recent Activities

The research on smart environments is ongoing. We will continue to develop our smart environment for DDL further.
Through various hackathons we try to identify common steps to build smart environments. The objective is to achieve a process-based understanding Students in the Masters program [Services Computing](http://www.hhz.de/master/services-computing/) attending my elective course Internet of Things (IoT) will actively participate in this endeavor. 

Another branch of research is the investigation of big data and machine learning approach to efficiently process and reason on the data acquired by the embedded sensor systems. 

Finally, the use of peripherial displays and other actuators to let the environemnt *interact* with people, is wide area of research we will explore.

Recent activities are reported in the articles below.

* T. Strobl, State Minister of the Interior visits HHZ, [Tweet](https://twitter.com/cdeck3r/status/880786015845273600)
* June 2017, SCM Hackathon, [blog post & projects](http://cdeck3r.com/2017-06-13-SCM-IoTHackathon/)
* January 2017, SCM Hackathon, [blog post](http://cdeck3r.com/2017-01-18-SCM-IoTHackathon/)

## Collaboration

If you are interested to collaborate in our activities, do not hesitate to contact me.