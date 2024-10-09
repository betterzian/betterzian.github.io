---
title: 'Extensive Form Games （扩展形式博弈）'
date: 2024-10-01
permalink: #/posts/2014/08/blog-post-3/
tags:
  - Game Theory
---


including: Extensive Form Games

Extensive Form Games （扩展形式博弈）
======

***Def:*** multi-agent sequential decision making - multiple players generally make decision one by one.

- All previous action are observed.
- Some players may move simultaneously at some stage k.

Extensive form games can be represent as  a game tree.

## Extensive Form games with perfect information

- **perfect information**: When moving, each player is aware of the previous moves.

- Players do not move simultaneously.

- A (pure) strategy for player $i$ is a mapping from player $i$'s nodes to actions.

### game model

- A set of players, $N=\{1,\dots,I\}$

- Histories: A set $H$ of sequences which can be finite or infinite.

  $h^0=\emptyset$                                    initial history

  $a^0=(a_1^0,\dots,a_I^0)$                 stage 0 action profile

  $h^1=a^0$                                  history after stage 0

  $\cdots$

  $h^{k+1}=(a^0,a^1,\dots,a^k)$      history after stage k

- If the game has a finite number (K+1) of stages, then it is a finite horizon game.

- Let $H^k=\{h^k\}$ be the set of all possible stage k histories.

- **Terminal history**: Then $H^{K+1}$ is the set of all possible terminal histories.

- **Terminal history set**: $H = \cup_{k=0}^{K+1}H^k$ is the set of all possible histories.

**Pure strategies** for player $i$ is defined as a contingency plan for every possible history $h^k$.

- Let $S_i(H^k)=\cup_{h^k\in H^k}S_i(h^k)$ be the set of actions available to player $i$ at stage $k$.
- Let $s_i^k:H^k \rightarrow S_i(H^k)$ such that $s_i(h^k) \in S_i(h^k)$.
- Then the pure strategy of player $i$ is the set of sequences $s_i=\{s_i^k\}_{k=0}^K$.
- Observe that the path of strategy profile $s$ will be $a^0=s^0(h^0)$, $a^1=s^1(h^1)=s^1(a^0)$,$a^2=s^2(h^2)=s^2(a^0,a^1)$, and so on.

**Payoff** of player $i$ is represented by $u_i:H^{K+1} \rightarrow R$.

### Conversion from extensive to normal form

***Example:***

![image-extensive1](./../assets/post/image-extensive1)

![image-extensive2](./../assets/post/image-extensive2)

We can find the Nash equilibria: (In,A), (Out,F).

However, The player "Entrant" chooses "In" would always get the higher reward if the player "Incumbent" is rational enough to choose A. That means (Out,F) is sustained by a **noncredible** threat of the monopolist.

To solve that problem, we will introduce subgame perfect equilibrium.

### Kuhn Theorem

**In the games with perfect information, for every mixed strategy there is a behavioral strategy that has an equivalent payoff.**

### Subgame Perfect (Nash) Equilibrium

It is an equilibrium notion for extensive form games.

- It requires each player's strategy to be "optimal" not only at the start but also after every history.
- For finite horizon games, found by **backward induction（诱导策略式博弈）**.

### backward induction

When we know what will happen at each of a node's children, we can decide the best action for the player who is moving at that node.

But if there are equally probable, then it may be depend on casing.

![image-extensive3](./../assets/post/image-extensive3)

## Extensive Form games without perfect information

Not yet.
