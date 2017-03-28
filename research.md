---
title: "Hydro-Turbine Optimization"
author: Richard Xu, Matt Chodazcek, Allie Farrelly, Eric Xue
date: March 27 2017
output: pdf_document
---

# Introduction
This is a panda

![The Victim](https://media4.s-nbcnews.com/j/newscms/2016_36/1685951/ss-160826-twip-05_8cf6d4cb83758449fd400c7c3d71aa1f.nbcnews-ux-2880-1000.jpg)

## Intro
Settled by Thomas Fowler in 1829, Maine became a hub the Through an analysis of the changing state of hydro-electric power in the of Millinocket, Maine.  

$f(x) = sin(x) + 12$

```mermaid
graph LR
A --> B
B --> C
```
## Problem 1
$f(Q_{1}, Q_{2}, Q_{3}) = KW_{T} = KW_{1} + KW_{2} + KW_{3}$

$g(Q_{1}, Q_{2}, Q_{3}) = Q_{T} = Q_{1} + Q_{2} + Q_{3}$

$\Lambda\ \nabla\ g = 3$

$K_{TQ_{1}} = \Lambda$ $K_{TQ_{2}} = \Lambda$ $K_{TQ_{3}} = \Lambda$   

$\therefore K_{TQ_{1}} = K_{TQ_{2}} = K_{TQ_{3}}$

Now

$KW_{T} = ((-18.89 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 ) + (-24.51 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2) + (-27.02 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2))(170 - 1.6\cdot{10^{-6}}Q_{T}^2)$

$KW_{TQ_{1}} = ((70.42 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2) + (1.6*{10^{-6}})$
