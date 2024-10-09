---
layout: archive
title: "Experiences"
permalink: /experiences/
author_profile: true
# redirect_from:
#   - /resume
---

{% include base_path %}

1、Terminal Cloud Service Business Feature-Aware Scheduling Technology
=====
* The main person in charge  
* Sep 2022 - Present  
* Nanjing, Jiangsu  
* Huawei Technologies Co., Ltd. | Southeast University  
* Project Overview:  
  Many companies deploy services provided to end-users in container form on cloud service providers for long-term periods. These services experience tidal effects in resource usage, with low server resource utilization during off-peak times. To improve resource utilization, cloud service providers introduce short-term services like machine learning tasks to these servers.  
* Main Responsibilities:   
  1. Propose an automatic path-aware heuristic method using Markov chains and topological relationship graphs to establish state transition matrices, and identify call chains based on changes in request arrival rates.   
  2. Propose a path-aware scale-in/scale-out algorithm to handle surges in request volumes.   
  3. Utilize graph convolutional networks and LSTM models combined with reinforcement learning algorithms to automatically select the appropriate resource usage to meet the task's SLO constraints.  
* Project Outcome:  
  Expected to win the Huawei Spark Award.  


2、Kubernetes scheduling algorithm optimization
=====
* The main person in charge  
* Jan 2023 - Present  
* Nanjing, Jiangsu  
* China Aerospace Science and Industry Corporation 8511 Institute | Southeast University  
* Project Overview:  
  The native scheduling algorithm of Kubernetes is a scoring algorithm primarily aimed at load balancing, while server cluster providers are keen on improving resource utilization.  
* Main Responsibilities  
  1. Read the Kubernetes scheduler source code to understand the Kubernetes scheduler extension interface and how to extend it.  
  2. Propose a vector distance-based heuristic algorithm to improve resource utilization.  
  3. Coordinate the tasks for implementing the algorithm.  


3、Optimization of Distributed IP Address Collision Prevention Allocation Algorithm
=====
* The main person in charge  
* Sep 2021 - Jun 2022  
* Nanjing, Jiangsu  
* Huawei Technologies Co., Ltd. | Southeast University  
* Project Overview:  
  In a certain area, all base stations can allocate IP addresses to users, but when a user moves to another base station, the new base station must reallocate a non-duplicate new IP address to avoid address collisions. This project aims to reduce the overall probability of collisions.  
* Main Responsibilities:  
  1. Abstract the problem into a mathematical model and propose using vertex coloring.  
  2. Propose a distributed vertex coloring algorithm to reduce the number of communications between base stations and decrease the number of colors needed for coloring.  
  3. Establish a new IP data structure that ensures a zero collision probability during idle times and reduces collision probability during busy times.  
  4. Write Python simulations for experiments and submit the final C code for use.  
* Project Outcome:  
  Huawei tested the new algorithm using historical data from base stations in the Tianhe District of Guangzhou, successfully reducing the collision probability from 11% to 1%.  
  simple code can be seem at [github](https://github.com/betterzian/IP).  

<!-- Work experience
======
* Spring 2024: Academic Pages Collaborator
  * Github University
  * Duties includes: Updates and improvements to template
  * Supervisor: The Users

* Fall 2015: Research Assistant
  * Github University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub

* Summer 2015: Research Assistant
  * Github University
  * Duties included: Tagging issues
  * Supervisor: Professor Git -->
  
<!-- Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3 -->

<!-- Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
   -->
<!-- Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams -->
