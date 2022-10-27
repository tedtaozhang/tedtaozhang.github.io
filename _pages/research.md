---
layout: archive
title: ""
permalink: /research/
author_profile: true
redirect_from:
  - /projects
---

{% include base_path %}

Current Projects
====

Control Scheme in Swarm Operations Based on Game Theory
---
In a swarm competition scenario, the real-time decision-making problem in terms of task assignment and motion control is hard to address. For example, two groups of intelligent agents, which have different goals in a non-cooperative environment, are seeking proper control schemes to make reliable decisions. 

I applied the matrix-game-based model and developed a fast and optimal search algorithm to solve the decision-making problem. More specifically, I applied the Action-Reaction Search (ARS) method to find the Nash equilibriums in a large-scale payoff matrix without calculating the matrix's all elements. Besides, the target assignment problem involved was solved by using a classic maximum weighted matching algorithm - the Kuhn-Munkres algorithm.
<div>
<img src='/images/project-result-cpu-time-an-optimal.png'>
<img src='/images/project-result-trajectory-an-optimal.png'>
</div>
It's difficult to find optimal solutions all the time - sometimes we just need to obtain a not-so-bad outcome. And that is what game theory can bring to us: it guarantees a optimal result under worst cases. By applying the matrix game, however, another issue came - the combination of agents' strategies became so large that the Nash equilibriums couldn't be computed in a short period. ARS solved such a problem through alternating row and column search and Nash equilibriums can be calculated quickly.

Something interesting: I was walking alone the night before we found the ARS, thinking about the solution to the problem. With a flash of inspiration, I came up with a search method and then verified its effectiveness. However, when I read a thesis a few days later, I surprisingly found that the ARS method in this article was identical to my idea.
