---
title: 'Cournot Model of Duopoly（古诺双寡头模型）'
date: 2024-10-01
permalink: #/posts/2014/08/blog-post-3/
tags:
  - Game Theory
---


including: Cournot Model of Duopoly

Cournot Model of Duopoly（古诺双寡头模型）
======

***Example:*** 

- $n$ number of ISPs offer their serivice (Bandwidth) to the customers.

- The cost to ISP $i$ of producing $q_i$ units of the Bandwidth is $C_i(q_i)$, where $C_i$ is an increasing function.
- The Bandwidth is sold at a single price $P(Q)$ where $Q$ is the total output and $P$ is a decreasing function unless it is already zero.
- If the output of each lSP $i$ is $q_i$, then the price is $P(q_1+\dots+q_n)$, so revenue of $i$ is $q_iP(q_1+\dots+q_n)$
- Thus ISP $i$'s profit, equal to its revenue minus its cost, is
  $$F_i(q_1,\dots,q_n)=q_iP(q_1+\dots+q_n)-C_i(q_i)$$
- The lSP Games:
  - Players: the lSPs.
  - Actions: the set of its possible outputs $q_1,\dots,q_n$.
  - Utilities: ISPs preferences are represented by their profits $F_1,...,F_n$.

***Processing:***

Every ISP wants to get maximum value of $F_i(q_1,\dots,q_n)$, then for each $i$, there is $\frac{\partial F_i}{\partial q_i}=0$. At last, we can get $q_i$ by these formula.

