---
title: 'Repeated Games（重复博弈）'
date: 2024-10-01
permalink: #/posts/2014/08/blog-post-3/
tags:
  - Game Theory
---


including: Repeated Games

Repeated Games（重复博弈）
=====

A player may be repeat play the game with the same rival.

A player may be deterred from exploit his short-term advantage by the "threat" of "publishment" that reduces his long-term payoff.

![image-repeated1](./../assets/post/image-repeated1)

Suppose that a player adopts the **grim trigger strategy**:

- Choose C so long as the other player chooses C;
- If in any period the rival chooses D, then choose D in every subsequent period.

Then, choosing C is the best response.

## Discount

The reasons for needing discount future payoffs:

- The game might stop in any round with some probability $1-\delta$.

- Payoffs in the future are worth less due to inflation or because gains received now can be invested.
- In an infinitely Repeated Game, define the utility as the sum of all periods would make the payoff unbounded.

Given a discount factor $\delta \in (0,1)$, then player $i$ obtains the utility $u^t_i = \delta^tu^t_i$ in the time period $t$. Then the total utility for history action $h=(a^0,a^1,a^2,\dots)$ is $$u_i(h)=\sum^{\infty}_{k=0}\delta^ku_i(a^k)$$, 

where $a^k=(a^k_1,a^k_2)$ is the set of actions for all players at time $k$.

## When will the player deviate?

If player 1 and 2 always choose C, the utility of player 2 is:

$$u_2(h)=\sum^\infty_{t=0}\delta^tu(a_2^t)=2+2\delta+2\delta^2+\dots=\frac{2}{1-\delta}$$

If player 2 adopts a different strategy, there is at least one period in which she chooses D, then player 1 chooses D in the next all periods until the end which force the player 2 to choose D forever since D is his unique best response to D. In that case, the utility of player 2 at the period he adopts the different strategy is:

$$u_2(h)^{'}=\sum^\infty_{t=0}\delta^tu(a_2^t)=3+\delta+\delta^2+\dots=2+\frac{1}{1-\delta}=\frac{3-2\delta}{1-\delta}$$ 

So the player 2 cannot increase his payoff by deviating if and only if $$u_2(h)\geq u_2(h)^{'}$$, then $\delta \geq \frac{1}{2}$.