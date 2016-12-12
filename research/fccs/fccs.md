---
layout: minimal
title: Feedback Controlled Computing systems
subtitle: Cooperation and Collaboration for Ubicomp
---

The study of feedback controlled computing systems led to a new theory of cooperative and collaborative process organisation.
It finds it application on resource constrained, embedded, ubiquitous computing platforms, e.g. the [Particle platform](http://particle.teco.edu). 
The research topic was part of the my dissertation.

Dissertation download: [diss_decker_final1.pdf](http://www.teco.edu/~cdecker/projects/fccs/diss_decker_final1.pdf)

## Synopsis

In unknown environments, data processing on miniaturized sensor and computer systems may lead to runtime-variant process behavior affecting the overall system performance. Feedback controllers allow to monitor the computer system online and adjust runtime parameters for achieving a pre-defined behavior. The objectives are to ensure fairness among processes, avoid system overload, coordinate realtime and non-realtime processes, form collaborative communication groups among nodes and and enable the best possible achievement for a demanded battery lifetime.
Theory of cooperative and collaborative process organisation

In data processing we observe two types of behaviors during execution: (1) processes affecting each other and (2) jointly interacting processes. We define the process behavior as follows:

* Cooperation: Goal oriented co-action of independent processes.
* Collaboration: Goal oriented interaction between dependent processes.

## Model

We model a process as an impact on a resource. Typical resources are for instance energy or message buffers. The resource is also called a budget. From this perspective, the previous definition of cooperation and collaboration is understood in the following way:

* Cooperation: direct impact on the budget by means of a process execution, e.g. energy consumption
* Collaboration: indirect impact on the budget by a process execution as a result of an interaction between processes, e.g. message exchange

Because of conservation, the budget is modelled as an integrator, i.e. every budget usage adds to the previous one. The usage of the budget is affected by the process organisation. This is the input to the budget. It is referred to it as cost. The goal is to achieve a defined overall budget usage after several iterations. This could be for instance an achieved system utilization, energy consumption or message buffer throughput. During the runtime the budget is fed back and compared with the setpoint. The process organisation is adjusted to affect the budget in a way that the setpoint can be achieved.

This relationship is expressed in the budget/cost control loop, which is shown in the picture below.

Budget/Cost control loop

The budget/cost control loop implements the separation of concerns principle. The unknown process behavior, e.g. execution time or energy consumption of a stateful sensor sampling process, can be thought of as the disturbance effect in this picture. The model separates between an ideal process execution behavior overlayed by an unknown disturbance.
Insight

The control approach has two behaviors, which can be derrived analytically from control theory: reference control, disturbance control.

Reference control: a given setpoint is achieved through a controlled process organisation.
Disturbance control: a disturbance during the process execution can be compensated.
Both behaviors are shown in the pictures below.
Control loop behavior

The gained insight is that:
    If a process organisation can be described by means of the budget/cost control loop, it shows the goal oriented process behavior of cooperation and collaboration.

As a result, a novel theory of cooperative and collaborative process organisation is established. 
It is not neccessary to concretly know the implementation of the process, i.e. what the process does. It is required that a process is part of a specific process class indicating it's timely behavior. So far, the theory was applied to periodic, aperiodic, realtime and distributed process classes.

## Results

For different types of processes commonly used on embedded ubiquitous computing systems, 
it was shown that cooperation and collaboration significantly improve the system's performance and 
hold guarantees. Novel forms of cooperative and collaborative process organisation as concrete 
instances of the budget/cost control loop for each process class were found. 

For instance: Fair Quality Scheduler (FQS), Buffer Feedback Scheduler (BFS), 
Feedback Controlled Unsynchronized Periodic MAC (FCUP-MAC) and others enable 
a more efficient resource usage than comparable approaches. Further, cooperative behavior 
allows to a achieve best an given operation duration of a battery driven ubiquitous computing system.

Other improvements were demonstrated in ubiquitous computing appliances, such as [RemCam](http://www.teco.edu/~cdecker/pub/decker_ucs2006.pdf) 
and [CoBIs](http://www.teco.edu/~cdecker/cobis/), and other experimental setups and simulation studies. 
A consistent view on theory, simulation and experiements was shown.

Process 	Control action 	Organisation 	Achievments
Periodic 	FQS 	cooperative, collaborative 	prompt data processing of all processes, novel operating system Particle OS
Aperiodic 	controlled M/D/k/k 	cooperative 	fair event processing, avoiding overload
Realtime 	BFS 	collaborative 	coordination of realtime with non-realtime processes, overall system speedup >2x, optimal utilization
Distributed 	FCUP-MAC 	collaborative, cooperative 	32% less latency, up to 10x more successfully exchanged messages, equalizing energy capacity levels
Energy management 	PControl 	cooperative 	a given operation duration (battery lifetime) is achieved best

## Relation to Ubicomp

In Ubiquitous Computing (Ubicomp), the complexity of working with a multitude of devices surrounding the user changes by embedding them into the environment (see figure below). The user cannot distinguish between single devices and is only aware of available services. The complexity becomes a complexity of data processing (= software) on and between devices. We propose to organize this processing along the control mechanisms of cooperation and collaboration.

IMG: ubicomp environment
Fig. In Ubicomp, the device usage complexity moves into the background and becomes a data processing complexity. (Source: Philips Research)

In order to find appropriate control setpoints for the budget/cost model, we introduce the principle of prompt data processing.
It says: As soon as data is available for a process to start, it should process them. 
This principle is useful in the Ubicomp user/environment relationship, because the user expects the services to behave timely to his/her actions.
A derived setpoint could be an execution priority, message buffer throughput or system utilization for achieving prompt data processing. It always applies to all processes of one class. Some examples:

* all periodic processes should achieve an overall fair execution priority despite unavowedly changing process durations, which delay start times of subsequent processes.
* all aperiodic processes should process events with an common event omission probability (dependent on the respective event rate) in order to achieve a defined system utilization and to avoid overload.
* all distributed processes support message forwarding to inactive stations by storing them up to a specific fill level in their message buffer.

**Note:** Prompt data processing differs from ASAP scheduling, because processes are non-preemptive complex software entities which run to completion. Prompt data processing only applies when a process starts. It does not apply during its execution.

The prompt data processing principle turned out to be extremely fruitful. It avoids overload and balances the resource usage between non-preemptive processes (cooperation). It speeds-up coordination among distributed and realtime/non-realtime processes (collaboration). Data processing could be dynamically prioritized, e.g. when starvation impends. On the other hand, it provides flexibility to the developer in prioritizing certain processes, e.g. data sampling for a specific sensor.

## Limitations and Extensions

The feedback control approach is currently limited to a SISO system considering only the effect on one control variable on one budget. A useful extension would be to go for MIMO systems, where multiple control variables and effects can be considered.

Definitely, it is interesting to identify, e.g. by means of system identification, the effects of data processing on resources in dependence of input data. Hidden states in the data processing software, its natural non-linear behavior and limited computing and memory resources of Ubicomp devices make this topic a big challange. However, solving those difficulties could result in cooperation and collaboration behavior profiles, which allow a very fine-tuned resource usage adaptation in unpredicatable environments.

Finally, established tool chains for system analysis and control synthesis, e.g. Matlab, can now be combined more deeply with model driven software development approaches, e.g. Eclipse modelling tool chain.
Further Readings

Decker, C.
*Prozessorganisation in eingebetteten, ubiquitären Rechnersystemen*
PhD thesis (German), University of Karlsruhe, 2009.[pdf]
Abstract(German): [[pdf]](http://www.teco.edu/~cdecker/projects/fccs/diss_abstract.pdf)
Presentation(German): [[pdf]](http://www.teco.edu/~cdecker/projects/fccs/disputation_cdecker_final.pdf)

Decker, C., Beigl, M., Riedel, T., Krohn, A., Zimmer, T.
*Buffer Feedback Scheduling: Runtime Adaptation of Ubicomp Applications*
International Symposium on Ubiquitous Computing Systems (UCS 2006) Oct. 11 - 13, 2006, Seoul, Korea, Lecture Notes in Computer Science (LNCS), Vol. 4239, Springer Verlag, 2006, ISBN 3-540-46287-2 [pdf]

Introdcutional course from Chenyang Lu
*Feedback Control Theory from a Computer System Perspective*
Department of Computer Science, University of Virginia [ppt]

Joseph L. Hellerstein (Author), Yixin Diao (Author), Sujay Parekh (Author), Dawn M. Tilbury
*Feedback Control of Computing Systems*
Wiley-IEEE Press (August 24, 2004), ISBN-13: 978-0471266372 
