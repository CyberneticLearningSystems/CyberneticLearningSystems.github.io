---
layout: default
title: A Novel Framework for Complex DJSP with Reinforcement Learning
description: Master Thesis - Julia Usher, January 2023 - August 2023
---

The low profit margins and highly cyclical nature of the aviation industry and affiliate industries makes the costs 
associated with delays and the propagation thereof severe, leading to significant research into understanding the 
root causes and the development of prediction networks, early-warning systems and robust systems. Ground handling 
agents are unique aviation stakeholders, given the scope of the work they do and the required skillset. Ground 
handling operations consist of a multitude of intricate and codependent processes, requiring a fleet of specialised 
equipment and well-trained staff. Given that on-time-performance is one of the key performance indicators for ground 
handling agents, there is significant interest in designing their operations to prevent delay generation and absorb 
the effects of incoming delays. 

This thesis delves into the world of scheduling using Reinforcement Learning (RL), developing a proof-of-concept for 
the scheduling of ground handling equipment to flights using RL, a small cog in the larger monitoring, simulation 
and AI-driven recommendation system being developed for Swissport in the [brAIght](./../projects/braight.md) project.

A Dynamic Job-shop Scheduling Problem (DJSP) formulation of the ground handling equipment (GHE) scheduling task was 
developed and a custom RL environment developed to generate solutions. Variable instance parameters allow the developed 
model to be highly customisable. The RL agent was trained and tested using custom-generated instances of various 
sizes and complexity (for example Figure 1), considering both parallel and sequential process interdependencies are 
considered, a novelty within the field of the DJSP. 

![Branching](./../../pictures/mt_julia_usher_operation.png)
_Figure: An example of a test process with 8 subprocesses, three parallel branches, two of which contain 
sequentially dependent operations._

The RL agent was quickly able to perform simple scheduling tasks, proving the potential of applying RL to the DJSP. 
While the agent initially struggled to schedule larger and more complex problems in an optimal manner, further 
development put it on a trajectory of improvement and a detailed analysis of the learning curves and model parameters 
shed light on areas requiring further work and was able to provide learnings for continued development. 

[Back](https://cyberneticlearningsystems.github.io/pages/research.html)