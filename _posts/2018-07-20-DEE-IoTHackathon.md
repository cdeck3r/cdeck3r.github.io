---
layout: post
title: Cross-Education Project on Blockchain   
subtitle: Distributed Economy and IoT Hackathon Summer 2018
share-img: "http://cdeck3r.github.io/img/blog/DEE_IoT_SS18_Hackathon.jpg"
bigimg:
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg1.jpg" : "Students from both departments discussion the solution (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg2.jpg" : "Review and understanding of the load simulation (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg3.jpg" : "Statistics on blockchain's operation (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg4.jpg" : "The blockchain operates  properly (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg5.jpg" : "Whiteboard modelling and design (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg6.jpg" : "Pen, paper, food, drinks for a better discussion (2018)"
  - "/img/blog/DEE_IoT_SS18_Hackathon_bigimg7.jpg" : "Presenting the development activities (2018)"

---

We brought together our computer science students from the IT Master program [Services Computing](http://www.hhz.de/master/services-computing/) with the students from the electrical engineering department at the Reutlingen University. In a 2-day hackathon on July 5/6, 2018 they have implemented a prototype blockchain based P2P transactions for an energy microgrid. See the video below to get an impression on the solution they came up. The teams' docs: [Team 1](https://hsrt.gitbook.io/dee-scm/), [Team 2](https://hhz.gitbook.io/blockchain/)

**Video:**
<div id="yt_embed_1" width="560" height="315"><a class="youtube"><img id="1" src="/img/blog/DEE_IoT_SS18_Hackathon_yt_preview.jpg" alt="Blockchain based P2P transactions in energy microgrid, DEE IoT Hackathon" width="560" height="315" /></a></div><script type="text/javascript">document.getElementById('yt_embed_1').onclick=function(){if(confirm("If you accept this message box by clicking OK, the Youtube video will load. Youtube will record your personal access related data and set a cookie in your browser. ")){var c = document.getElementById('1'); c.parentNode.removeChild(c); document.getElementById('yt_embed_1').innerHTML += '<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/yWSbyTVmJwM?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>';}else{alert("You find the video on //youtu.be/yWSbyTVmJwM");}}</script>

## Background 

[Prof. Coll-Mayor](https://www.tec.reutlingen-university.de/fakultaet/personen/professoren/#debora-coll-mayor) and [Prof. Notholt](https://www.tec.reutlingen-university.de/fakultaet/personen/professoren/#antonio-notholt) research energy microgrids. Therein, energy consumers and producers relate their energy haves and needs with each other. Running such a grid without a central authority provides an valuable mode of operation, where participants execute transactions in a P2P manner. 

[My research focus](/research) is the Internet of Things (IoT). Primarily, in the Internet of Things (IoT), Smart Data Services become business relevant first-class resources and enable new business models. As a result, Data Products emerge where products and services embodying data intelligence provide novel value propositions to the user.

## Motivation and Goal

By enabling energy producers and consumers to act locally with each other in a microgrid utilizing smart software services running directly on inter-connected things or devices, we are able transform physical resources into first-class business objects. 

We believe novel applications will stem from this approach and we want to establish a [laboratory environment](https://dlt-lab.reutlingen-university.de) at the Reutlingen University to study and develop these applications.

Our goal is support research and teaching on IT based physical business objects.

## Lecture and Research 

[Smart Contracts on Blockchain](http://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/smart_contracts_2.html) may offer an potential technology to implement P2P  transactions in energy microgrids. 

Students from both, computer science and electrical engineering departments, worked together to learn about the blockchain approach and apply them in a prototype implementation of a microgrid scenario.

First, they attended the lecture on Distributed Energy Economy given by Prof. Coll-Mayor. They learned about microgrids, the various stakeholders and their business and technical relations with each other. Several lab exercises have taught them the fundamentals in the technical principles of blockchain as well as the programming of Ethereum smart contracts using [Solidity](https://github.com/ethereum/solidity). 

## Hackathon

> **Hackathon's objective:** to demonstrate the technical feasibility of blockchain based P2P transactions in a energy microgrid use case.

The basic setting provided simulated loads by a photovoltaic system, battery, combined heat and power unit. Raspberry Pi embedded computers made up the IoT part for building a device network executing smart contracts between the network participants. 

The students were split into two teams. In both teams computer science students as well as electrical engineering students took part. Using UML modelling diagrams they were quickly able to achieve a common understanding on their envisioned prototype design.

The teams came up with different solutions concepts:

* P2P transactions between the network participants using a single smart contract. It basically works like a market place.
* A single smart contracts for each network participant. In this concept several smart contracts interact with each other.

![Students working in the hackathon](/img/blog/DEE_IoT_SS18_Hackathon_students.jpg)

It was impressive to see how students from different departments worked together - a true cross-educational endeavour. 

## Resources

My students have compiled a comprehensive documentation available on as [gitbook](https://www.gitbook.com/). Check out their material.

* [Hackathon Team 1](https://hsrt.gitbook.io/dee-scm/)
* [Hackathon Team 2](https://hhz.gitbook.io/blockchain/)

