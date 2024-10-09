---
title: "OneMore: Task Colocation Scheduling in Heterogeneous Clusters"
collection: publications
categories: 
    - manuscripts
permalink: /publication/OneMore_Task_Colocation_Scheduling_in_Heterogeneous_Clusters
excerpt: 'Has been prepared by Authors: ___Zian Yuan___, Shuang Wang&dagger;, Xin Li,  Jinquan Zhang, Xiaoping Li&dagger;'
date: 2024-10-01
venue: 'None'
slidesurl: #'http://academicpages.github.io/files/slides2.pdf'
paperurl: #'http://academicpages.github.io/files/paper2.pdf'
citation: 'Not yet.'
---

The increasing deployment of online tasks to handle user requests faces fluctuating resource requirements, leading to underutilization. To address this, offline tasks are deployed on the same servers as online tasks, known as colocation. How to schedule these tasks to suitable resources is difficult. Additionally, when servers lack resources, any running offline tasks will be terminated, resulting in the used resources being wasted. In this paper, the OneMore algorithm is proposed to improve resource utilization, including the resource shaping algorithm which smooths online task resource fluctuations by processing offline tasks to reduce waste and the double gated greedy state value algorithm which seeks to optimize the placement of offline tasks on servers. Through an analysis of variance, the performance of parameters on the algorithm is evaluated. By comparing OneMore to the other six algorithms across numerous instances, the experimental results demonstrate the superiority of others consistently.

Code can be got at [github](https://github.com/betterzian/OneMore).