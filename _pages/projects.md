---
layout: page
title: research
permalink: /research/
description: A growing collection of research projects that I have or are currently working on.
---

---
# Interests

As a computer scientist, I am always amazed by how much of technology is inspired by the biological phenomena seen in nature.
When we go outside and see all the complex life in nature today, it can be easy to forget that it all evolved from a single cellular organism.
Organisms on this evolutionary journey constantly faced new challenges, and evolution played an important role in an organisms’ ability to overcome these challenges and perform complex tasks.
Hence, it would seem that incorporating an evolution like framework within technology could be helpful.

My research interests fall at the intersection of computer science and biological evolution --- evolutionary computation.
I am interested in discovering the many strengths, weaknesses, and capabilities of different evolutionary algorithms.
Understanding these categories can potentially lead to the discovery of more robust algorithms.
I am also interested in exploring evolutions ability to construct more robust evolutionary algorithms.

#### Jump To
* [Selection Scheme Components](#ssc)
* [Selection Scheme Diagnostics](#ssd)

---
### <a name="ssc">Selection Scheme Components</a>

The field of evolutionary computation consists of a set of algorithms that take inspiration from different aspects of biological evolution.
Algorithms that fall under evolutionary computation explore and answer different kinds questions: from exploring and modeling phenomena seen in nature, to solving complex engineering problems that exist in the world.
There also exists a subset of algorithms within the field of evolutionary computation that focus on solving optimization problems --- evolutionary algorithms.

<div class="img_row">
  <img class="col two" src="{{ site.baseurl }}/assets/img/ssd.jpg" style="display: block; margin-left: auto; margin-right: auto; border: 7px solid #ddd; border-radius: 4px; ">
</div>
<div class="col three caption">
  In this project we focus on creating a conceptual framework to describe major components within a selection scheme.
</div>

Evolutionary algorithms are probabilistic search algorithms where evolutionary processes are used sample the space of possible solutions.
At any point in time, the set of candidate solutions under consideration is regarded as the population.
Each solution in the population is evaluated based on a given optimization problem to determine the set of solutions to act as parents for the construction of a new generation of solutions.
Offspring produced from the set of parent solutions will be subject to a source of variation, typically either mutations to their underlying representation or recombination with other parent solutions.

The previous description makes it clear that before an evolutionary algorithm can be executed, certain criteria, parameters, and procedures must be predetermined.
Some of these decisions include determining a solutions' underlying representation, mutation operators, selection scheme, stopping criteria, etc.
Having to describe every criteria, parameter, and procedure can make it difficult to understand and compare different evolutionary algorithms.
**This work hopes to help mitigate this issue by describing a conceptual framework to better describe selection schemes.**

A more formal description of this conceptual framework is coming soon!

---
### <a name="ssd">Selection Scheme Diagnostics</a>

Evolutionary algorithms are a great set of tools to use when it is not possible to represent an optimization problem in a clean mathematical formula and no assumptions about the fitness landscape are known.
The optimization problems that evolutionary algorithms attempt to solve possess characteristics that are common across other optimization problems; these characteristics are captured and represented by a set of diagnostics.
While different optimization problems may share certain characteristics, some are certainly harder than others.
Fortunately, these diagnostics will help describe an evolutionary algorithms strengths and weaknesses.

One major concern that arises when using evolutionary algorithms to solve an optimization problem is that it is very difficult to guarantee that an an optimal solution will be discovered.
This can happen for a variety of reasons, but a common one is due to the complex nature of the optimization problem.
An evolutionary algorithm has a number of components that interact during an evolutionary search, and each component plays an important role in the process of discovering an optimal solution.
In this work, the selection scheme is isolated to better understand its strengths and weaknesses.

<div class="img_row">
  <img class="col two" src="{{ site.baseurl }}/assets/img/ssc.jpg" style="display: block; margin-left: auto; margin-right: auto; border: 7px solid #ddd; border-radius: 4px; ">
</div>
<div class="col three caption">
  In this project we focus on understanding the strengths and weaknesses of different selection schemes.
</div>

The selection schemes of interest are evaluated against the set of diagnostics and copious data is collected.
This generates a *profile* for each selection scheme, and a profile reports information on the kinds optimization problems a selections scheme performs well against.
As previously mentioned, each component of an evolutionary algorithm plays an important role in the process of finding an optimal solution.
This work focuses on creating a framework to help provide information on the capabilities of different selection schemes, with the goal helping users make better decisions when constructing an evolutionary algorithm.

More information about this project can be found at [link](https://github.com/jgh9094/Selection-Scheme-Diagnotics-Part-I).
