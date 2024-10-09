---
title: 'Potential Games （势博弈）'
date: 2024-10-01
permalink: #/posts/2014/08/blog-post-3/
tags:
  - Game Theory
---


including: Potential Games and Congestion Games

# Potential Games （势博弈）

Introduce by [Cournot Competition](https://betterzian.github.io/Cournot_Model_of_Duopoly/):

- The payoff function for player $i$ given by $u_i(q_i,q_{-i})=q_i(P(Q)-c)$.
- Define a function $\Phi(q_1,\dots,q_I)=(\prod^I_{i=1}q_i)(P(Q)-c)$.     (1)
- Note that for all $i$ firms and all $q_{-i} >0$, $u_i(q_i,q_{-i})-u_i(q_i^{'},q_{-i})>0$ iff $\Phi(q_i,q_{-i})-\Phi(q_i^{'},q_{-i})>0$, $\forall q_i,q^{'}_i > 0$. 

A function $\Phi$ satisfying (1) is called an **ordinal potential**, and a game that possesses an ordinal potential is called an **ordinal potential game**. 
$q=(q_i,q_{-i})$ is an equilibrium point if and only if for every i, $\Phi(q_i,q_{-i})-\Phi(q_i^{'},q_{-i})>0$ for any $q_i^{'}>0$.

 A strategic form game is a **potential game** If there exists a **potential function** $\Phi:S\rightarrow R$ such that $\Phi(s_i,s_{-i})$ gives information about $u_i(s_i,s_{-i})$ for each $i\in I$.

## Formal Define

Let $G = <I,(S_i),(u_i)>$ be a strategic (matrix) form game, then ***Def***:

### ordinal potential function

A function $\Phi:S\rightarrow R$ is called an **ordinal potential function** for the game G if for each $i\in I$ and all $s_{-i}\in S_{-i}$, $u_i(x,s_{-i})-u_i(z,s_{-i})>0$ iff $\Phi(x,s_{-i})-\Phi(z,s_{-i})>0$, for all $x,z\in S_i$.

G is called an **ordinal potential game** if it admits an ordinal potential.

### $\omega$-potential game

let $\omega=(\omega^i)_{i\in N}$ be a vector of positive numbers which will be called **weights**.

A function $\Phi:S\rightarrow R$ is called an **$\omega$-potential function** for the game G if for each $i\in I$ and all $s_{-i}\in S_{-i}$, $u_i(x,s_{-i})-u_i(z,s_{-i})=\omega^i\Phi(x,s_{-i})-\Phi(z,s_{-i})$, for all $x,z\in S_i$.

G is called an **$\omega$-potential game** if it admits an ordinal potential.

### exact potential function

A function $\Phi:S\rightarrow R$ is called an **exact potential function** for the game G if for each $i\in I$ and all $s_{-i}\in S_{-i}$, $u_i(x,s_{-i})-u_i(z,s_{-i})=\Phi(x,s_{-i})-\Phi(z,s_{-i})$, for all $x,z\in S_i$.

G is called an **exact potential game** if it admits an ordinal potential.

## Theorem

**Every finite ordinal potential game has at least one pure strategy Nash equilibrium.**

## Improvement path

An improvement path is a path $(s_0,s_1,\dots)$ such that,

- $u_{i^k}(s^k)<u_{i^k}(s^{k+1})$ where $s^k$ and $s^{k+1}$ differ in the $i^k$th coordinate. In other words, the payoff improves for the player who changes his strategy.

- For a finite path $\gamma=(s_0,\dots,s_N)$, let $I(\gamma)=\sum_{i=1}^Nu^{m_i}(s^i)-u^{m_i}(s^{i-1})$, where $m_i$ denotes the player changing its strategy in the $i^{th}$ step of the path.
- The path  $\gamma=(s_0,\dots,s_N)$ is closed if $s^0=s^N$. It is a simple closed path if in addition $s^l \neq s^k$ for every $0\leq l \neq k\leq N-1$.

### Theorem

A game G is an exact potential game iff for all simple closed paths $\gamma$, $I(\gamma) = 0$. Moreover, it is sufficient to check simple closed paths of length 4.

# Congestion Games

***Example:***

![image-potential1](../assets/post/image-potential1)

## Define

Congestion Model: $C = <I,M,(S_i)_{i∈I},(c_j)_{j∈M}>$ where:

- $I = {1, 2,\dots,I}$ is the set of players.
- $M={1,2,\dots,m}$ is the set of resources.
- $S_i$ is the set of resource combinations (e.g., links or common resources) that player $i$ can take/use. A strategy for player $i$ is $s_i \in S_i$, corresponding to the subset of resources that this player is using. $c^j(k)$ is the benefit (the negative of the cost) to each user who uses resource $j$ if $k$ users are using it. 
- Define congestion game $<I,(S_i),(u_i)>$ with utilities $u_i(s_i,s_{−i})=\sum_{j\in S_i}c^j(k_j)$ where $k_j$ is the number of users of resource $j$ under strategy $s$.

## Theorem

**Every congestion game is a potential game and thus has a pure strategy Nash equilibrium.**

# References

1. [Monderer, D. and Shapley, L.S., 1996. Potential games. *Games and economic behavior*, *14*(1), pp.124-143.](https://www.sciencedirect.com/science/article/abs/pii/S0899825696900445)
2. [MIT-PPT](https://ocw.mit.edu/courses/6-254-game-theory-with-engineering-applications-spring-2010/71ac60209197560c1c3f3a5520bf8489_MIT6_254S10_lec08.pdf)