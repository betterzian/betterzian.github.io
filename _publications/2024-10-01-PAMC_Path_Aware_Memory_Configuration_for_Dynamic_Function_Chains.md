---
title: "PAMC: Path-Aware Memory Configuration for Dynamic Function Chains"
collection: publications
categories: 
    - manuscripts
permalink: /publication/PAMC_Path_Aware_Memory_Configuration_for_Dynamic_Function_Chains
excerpt: 'Has been prepared by Authors: Jinquan Zhang, ___Zian Yuan___, Xiaoping Li&dagger;, Yamin Lei, Long Chen&dagger;'
date: 2024-10-01
venue: 'None'
slidesurl: #'http://academicpages.github.io/files/slides2.pdf'
paperurl: #'http://academicpages.github.io/files/paper2.pdf'
citation: 'Not yet.'
---

Serverless applications based on microservices commonly comprise many loosely coupled functions. Each request in these applications triggers a function chain, the structure of which is a graph and may be dynamic due to the existence of conditional branches. Each function in the chain has multiple memory configurations, and the configuration space grows exponentially as the length of the chain increases. Therefore, it is challenging to determine the memory configurations for function chains with complex, uncertain structures and huge configuration spaces. This paper studies the memory configuration problem for dynamic function chains to minimize costs while meeting service level objectives. The proposed PAMC algorithm utilizes a recurrent neural network to track the invocation paths of function chains, employs reinforcement learning to choose memory configurations, and incorporates a two-stage feedback controller to meet the service level objectives. The PAMC algorithm is evaluated and compared to existing algorithms over many serverless applications. Experimental results show that PAMC significantly reduces the costs of dynamic function chains and outperforms other algorithms.