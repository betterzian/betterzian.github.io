---
title: 'Zero-sum Games（零和博弈）'
date: 2024-10-01
permalink: #/posts/2014/08/blog-post-3/
tags:
  - Game Theory
---


including: Repeated Games

Zero-sum Games（零和博弈）
=====

## Compuitation of Nash Equilibira of a Game

Depend on the class of games being considered

- compute the Nash equilibria of **simple games(two-player two-action game)**
- Linear programing solution for **simple two-player, zero-sum normal-form games**
- The Lemke-Howson algorithm for **general-sum normal-form games**

## Nash's THeorem

Every finite game(finite number of players, finitenumber of pure strategies) has at least one mixed-strategy Nash equilibirum.

## Minimax THeorem

For every two-person, zero-sum game with finitely many pure strategies, there exist a mixed strategy for each player and a value V such that:

- Given player 2's strategy, the best possible payoff for player 1 is V.
- Given player 1's strategy, the best possible payoff for player 2 is -V.

The existence of strategies part is a special case of Nash's theorem, and a precursor to it.

 It's called "minimax" because the players get this value by pursuing a strategy that tries to minimize the maximum payoff of the other player.

## Computing Nash Equilibria : 2-person, Zero-Sum Games

***Example:***

![image-zero1](./../assets/post/image-zero1)

Let $x_1$ denote the probability that player 1 plays action row1, then player 1 chooses row2 with probability $1-x_1$. So, the outcome that player 2 would get when he chooses col1 is $2x_1-3(1-x_1)$, when he choose col2, the outcome becomes $4(1-x_1)-3x_1$. If player 2 wants to get a higher value, $2x_1-3(1-x_1)$ must be equal to $4(1-x_1)-3x_1$, therefore $4(1-x_1)-3x_1 = 2x_1-3(1-x_1) \rightarrow 13x_1=7 \rightarrow x_1=\frac{7}{13}$. The computation of player 2 is similar to the computation before.

## Nash equilibria for zero-sum games in polynomial time

