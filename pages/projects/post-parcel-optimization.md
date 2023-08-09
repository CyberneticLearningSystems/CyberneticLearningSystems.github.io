---
layout: default
title: Swiss Post Digital Twin for Parcel Logistic Optimization
description: Research project in collaboration with Swiss Post to optimize parcel logistic on railway and road network
---

In cooperation with Swiss Post, our research group has developed a digital twin for the optimisation of parcel logistics on Swiss Post's rail and road network. The optimisation algorithm is based on a digital twin that was initially developed in two subsequent project works by Master students. The digital twin, which is based on discrete-event simulation, was further developed by Manuel Renold and his team. The model is now able to optimize the resource allocation of freight wagons across the Swiss Post rail fleet and trucks on the road. The combinatorial optimization algorithm solves the vehicle routing problem (VRP) using integer programming to find the globally best solution from the discrete set of all feasible solutions.

![Branching](./../../pictures/post_digital_twin.png)
_Figure 1: A cut-out of the model of the digital twin for the parcel logistics centre in Frauenfeld._

The digital twin model is already available as a prototype to test its ability to support the dispatcher in finding the optimal way to transport the parcel between the logistics centre in Frauenfeld and Härkingen. A GUI has been developed to allow the dispatcher to see the solution computed by the optimisation algorithm, to add constraints to the algorithm before it is re-run, and to test certain What-If scenarios by re-assigning transports at his request, with the digital twin in the background testing the consequences.

![Branching](./../../pictures/post_digital_twin_gui.png)
_Figure 2: Representation of the prototype's GUI to adjust the optimization algorithm and run What-If scenarios._

The digital twin model is designed in a modular way, which makes it possible to quickly add new logistics centres to build up the entire logistics network of Swiss Post and to test the economic and ecological benefits of investing in new logistics infrastructure. It is being considered to replace the existing combinatorial optimisation algorithm with new methods from the field of reinforcement learning, thus taking advantage of synergies from other projects such as the [Flatland Association](https://isandaiinaviation.github.io/2023-07-25-SBB-and-ZHAW-collaborating-in-Flatland.html).


### Acknowledgment

This project is based on a digital twin initially developed by two master's students in the first and second half of 2020, and since then continued by our research group with direct funding from Swiss Post.

[Back](https://isandaiinaviation.github.io/pages/research.html)