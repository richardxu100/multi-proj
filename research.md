---
title: "Hydro-Turbine Optimization"
author: Richard Xu, Matt Chodazcek, Allie Farrelly, Eric Xue
date: March 27 2017
output: pdf_document
---

# Introduction
Dating back to 1829, Maine was first settled by Thomas Fowler, along with his family. Shortly after inhabiting the area, he recognized its potential and opened it up to development. Charles W. Mullen, an engineering graduate from the University of Maine, hypothesized putting a dam on the Penobscot River in order to convert the water source into a power source. This dam would eventually be used to operate a large pulp and paper mill, Millinocket Paper Company. Then, on May 15, 1899, construction commenced. This remote location was set off from the rest of the island, hence the necessity to build a mill.

On March 16, 1901, Millinocket (meaning “the land of many islands”) was incorporated, jumpstarting the community. With most of the construction of Millinocket Mill being attributable to Italian masons, the community prospered. It rapidly developed a reputation as a small but successful rural town, mostly due to the paper industry. Coupled with the close proximity to Mount Katahdin, Maine’s tallest mountain, and Moosehead Lake, Maine’s largest lake, things were running smoothly.

Sadly, in early 2003, Great Northern Paper filed for bankruptcy protection for its Millinocket and East Millinocket mills. Ever since then, the mill town has struggled to revive its once thriving community.

Through the our applied project, we will optimize a hydro-turbine in Millinocket, Maine, facilitated by the Katahdin Paper Company. We will apply Bernoulli’s equations, as well as the given quadratic models.  


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

$\lambda\ \nabla\ g = \nabla <1, 1, 1> = <\lambda, \lambda, \lambda>$

$K_{TQ_{1}} = K_{TQ_{2}} =  K_{TQ_{3}} = \lambda$   

$\therefore K_{TQ_{1}} = K_{TQ_{2}} = K_{TQ_{3}}$

$\text{Let } a = 170 - 1.6\cdot{10^{-6}}Q_{T}^2$

$\text {Plugging in the question data, we find that: }$


$KW_{T} = ((-18.89 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 ) + (-24.51 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2) + (-27.02 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2))(a)$

$KW_{TQ_{1}} = ((-70.42 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2) + (1.6\cdot{10^{-6}}\cdot2(Q_{1} + Q_{2} + Q_{3})) + (.1277 - 8.16\cdot{10^{-5}}Q_{1})(a)$

$KW_{TQ_{2}} = ((-70.42 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2) + (1.6\cdot{10^{-6}}\cdot2(Q_{1} + Q_{2} + Q_{3})) + (.1358 - 9.38\cdot{10^{-5}}Q_{2})(a)$

$KW_{TQ_{3}} = ((-70.42 + .1277Q_{1} - 4.08 \cdot {10^{-5}}Q_{1}^2 + .1358Q_{2} - 4.69\cdot{10^{-5}}Q_{2}^2 + .1380Q_{3} - 3.84\cdot{10^{-5}}Q_{3}^2) + (1.6\cdot{10^{-6}}\cdot2(Q_{1} + Q_{2} + Q_{3})) + (.1380 - 7.68\cdot{10^{-5}}Q_{3})(a)$


$\text {Solving these equations, we find that:} $

$Q_{1} = .341Q_{T} - 75.174$
$Q_{2} = .297Q_{T} + 20.949$
$Q_{2} = .362Q_{T} + 54.225$

## Problem 2
$Q_{1} = .341Q_{T} - 75.174 \text { smallest when } Q_{T} \text { is small }$
$Q_{2} = .297Q_{T} + 20.949 \text { smallest when } Q_{T} \text { is large }$
$Q_{2} = .362Q_{T} + 54.225 \text { biggest always }$

$\text {Judging from the constraints listed, the smallest } Q_{T} \text { would be the one where the smallest } Q_{i} \text {was 250. }$

$\text {Using that information, we solved for } Q_{T_{min}} \text {, getting } Q_{T} = 953.589$

$\text {We used a similar process to discover } Q_{Tmax} \text {. The largest } Q_{i} \text {would be }  1225ft^3/sec \text { through turbine 3, meaning that } Q_{Tmax} \text { would be } Q_{T} = 3234.185 $

$\therefore 953.589 < Q_{T} < 3234.185$
