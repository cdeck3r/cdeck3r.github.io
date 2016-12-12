---
layout: page
title: CoBIs
subtitle: Collaborative Business Items 
---

Collaborative Business Items (CoBIs) is an EC funded project which bridges the gap between enterprise systems and networked embedded systems. Project partners are: SAP, Infineon, BP, TecO, Lancaster University, University of Twente and Ambient System.
Christian was the technical platform lead and represented TecO as the largest academic partner within the consortium.

### Synopsis

CoBIs researches the integration of wireless sensor networks in business processes. 
Our approach is to *bring parts of a business process to execution directly within sensor networks*.
Collaboration among the sensor nodes enables the execution of complex tasks and re-integrates the results in backend systems.

### Application

The following figures depicts an example of a CoBIs scenario for asset management and workplace safety in industrial environments. CoBIs nodes can collaborativly detect hazardous situations for chemical containments, e.g. wrong storage area, exceeded storage limit, incompatible (inflammable) combination of chemical containments.
In the example below chemical drums are represented by dummies. The CoBIs nodes detect whether the storage limit is exceeded or not. Hereby, no backend interaction is necessary. The CoBIs nodes on the drum replacements execute business logic and decide collaboratively about hazardous situation.
	
![CoBIs - storage limit ok](http://www.teco.edu/~cdecker/cobis/storage_limit_exceeded_green.jpg)   
Fig. Storage limit achieved (condition green)
	
![CoBIs - storage limit exceeded](http://www.teco.edu/~cdecker/cobis/storage_limit_exceeded_red.jpg)   
Fig. Storage limit exceeded (condition red)

At TecO we are working on capabable wireless sensor nodes ([Particle](http://particle.teco.edu) nodes) and a service-oriented architecture for integration. This approach results in an overarching concept since CoBIs employs not only one platform but many different. Apart from Particle Computer from TecO, the other platforms are Infineon's Sindrion platform and Ambient Systems µNodes. CoBIs can be applied in various scenarios. We especially investigate safety scenarios from BP involving storage of chemicals and worker safety. The approach can also be applied to electronic seals.
Finally, this CoBIs scenario was implemented in BP's chemical plant in Hull, UK. The following pictures illustrate the trial.

![CoBIs - Installation in Hull, UK](http://www.teco.edu/~cdecker/cobis/bp_hull1.jpg)   
Fig. CoBIs installation
	
![CoBIs - Installation in Hull, UK](http://www.teco.edu/~cdecker/cobis/bp_hull2.jpg)  
Fig. CoBIs Installation (close-up, CoBIs Particle Nodes)

Several trials were successfully conducted in 2006 and 2007.

### Technology

Requirements for a CoBIs technology are

* Sufficient computing power to execute business logic on the items
* Wireless communication capabilities to enables collaboration between business items and to organise distributed processes.
* Sensing capabilities for detecting item-to-item proximity and gathering environmental information
* Remote update for service deployment, i.e. moving business logic on the items, update and service reorganisation.
* Storage for services, but also for intermediate results, sensor data, tracking data, and logging

A possible instance of a CoBIs node is the DigiClip. 

![CoBIs node technical view](http://www.teco.edu/~cdecker/cobis/cobis_node_tech.jpg)   
Fig. CoBIs Node (DigiClip)

A second generation, CatPart, of nodes was develop including more sensors and a infrared (IR) location system packaged in a more robost housing for industrial trials. A photo of the hardware is shown on the right picture above.

![CoBIs node technical view](http://www.teco.edu/~cdecker/cobis/catpart_hw.jpg)   
Fig. CoBIs Node (CatPart)

### Results

CoBIs was successfully implemented for a period of several weeks in 2006 and 2007 in one of BP's chemical plant in Hull, UK.
By collaboratively updating the storage state of each service instance, storage regulations can be checked locally on each node. Local alarms are then also signalled collaboratively within a location. The hazardous situation due to storage violations was recognized within 1 second. According to BP up to 10 seconds are acceptable. In our experimental setting, flashing of the bright LEDs indicated the hazards. Clearly, the advantage is in-situ, real-time reaction by shortening the communication path and let the items directly reason on the situation without an permanent connection to a supervisionary backend system.
Relocated business logic utilizing collaboration among the sensor nodes keeps information local within the sensor network. Collaboration reduces the message load in case of hazardous detection events from 10 messages/s down to 2 messages/s. The complete history could be downloaded for instance during regular check or maintenance intervals.

### Further Readings

CoBIs demonstrators were successfully presented on SAPPHIRE 2005 in Copenhagen and Bosten and on DKOM 2005. The project was presented in detail in various SAP and BP magazines. CoBIs passed successfully the first review meeting March 2005.
A quick overview is presented in a flash video and a SAP TV appearance (Source: CoBIs website).

We successfully published several papers with more details on the CoBIs Architecture. Please refer to:

Decker, C., Riedel, R., Beigl, M., Moreira sa de Souza, L., Spiess, P., Haller, S., Müller, J.   
*Collaborative Business Items*   
Proceedings of the 3rd IET International Conference on Intelligent Environments (IE07), Sept. 24-25, 2007, Ulm Germany [pdf]

Riedel, T., Decker, C., Scholl, P., Krohn, A., Beigl, M.   
*Architecture for Collaborative Business Items.*   
20th International Conference on Architecture of Computing Systems, Zurich, Switzerland, Proceedings, Volume 4415 of Lecture Notes in Computer Science (LNCS). Springer, pp. 142-156, 2007. [pdf]

Decker, C., Spiess, P., sa de Souza, L.M., Beigl, M., Nochta, Z.  
*Coupling Enterprise Systems with Wireless Sensor Nodes: Analysis, Implementation, Experiences and Guidelines*   
Pervasive Technology Applied Real-World Experiences with RFID and Sensor Networks Workshop on Pervasive Technology Applied (PTA) at the International Conference on Pervasive Computing 2006, May 2006, Pervasive 2006 Workshop Proceedings, May 2006, ISBN 978-3-00-018411-6, pp. 393-400 [pdf]

Decker, C., Peev, E., Riedel, T., Berchtold, M., Beigl, M., Roehr, D., Beuster, M.  
*Using Auction based Group Formation for Collaborative Networking in Ubicomp*
International Symposium on Ubiquitous Computing Systems (UCS 2007) Nov. 25-28, 2007, Akihabara, Tokyo, Japan Lecture Notes in Computer Science (LNCS), Vol. 4836, Springer Verlag, 2007, ISBN xxx, pp.134-149 [pdf]

Decker, C., van Dinther, C., Müller, J., Schleyer, M., Peev, E.   
*Collaborative Smart Items*   
UbiLog @ Informatik 2007, Sept. 24-27 2007, Bremen, GI Proceedings 110, Band 2, ISSN 1617-5468, ISBN 978-3-88579-204-8 [pdf]

Decker, C., Riedel, T., Krohn, A., Berchtold, M., Beigl, M., sa de Souza, L., Spiess, P.  
*Collaborative Business Items*   
5th International Conference on Pervasive Computing, Toronto, Canada, In Advances in Pervasive Computing, Late Breaking Results, Austrian Computer Society, ISBN 978-3-85403-219-9, pp 33-36, 2007

Riedel, T., Decker, C., Berchtold, M., Beigl, M.   
*Life Cycle Management of Pervasive Services*  
5th International Conference on Pervasive Computing, Toronto, Canada, In Advances in Pervasive Computing, Late Breaking Results, Austrian Computer Society, ISBN 978-3-85403-219-9, pp 65-58, 2007

Please also check the consortium website on [www.cobis-online.de](www.cobis-online.de). 
