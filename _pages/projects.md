---
layout: page
title: projects
permalink: /projects/
description: A growing collection of research projects that I have or are currently working on.
---

---
# Intrests

As a computer scientist, I am always amazed by how much of technology is inspired by biological phenomena seen in nature.
When we go outside and see all the complex life in nature currently, it can be easy to forget that it all evolved from a single cellular organism.
Organisms on this evolutionary journey constantly faced new challenges that appeared, and evolution played an important role in an organisms’ ability to overcome these challenges and perform complex tasks.
So, it would seem that evolution would be a useful framework to incorporate within technology.

My research interests fall at the intersection of computer science and biological evolution --- Evolutionary Computation.
I am interested in discovering the many strengths and weaknesses behind different evolutionary algorithms.
Understanding these strengths and weaknesses can lead to the discovery of more robust evolutionary algorithms and a set of rules that different techniques maintain.
I am also interested in exploring if evolution has the ability to develop more robust evolutionary algorithms, as evolution tends to discover solutions that are unintuitive to human designers.

#### Jump To
* [Selection Scheme Components](#ssc)
* [Selection Scheme Diagnostics](#ssd)

---
### <a name="ssc">Selection Scheme Components</a>

The field of evolutionary computation consists of a set of algorithms that takes inspiration from different aspects of biological evolution.
Algorithms that fall under evolutionary computation explore and answer different kinds questions: from exploring and modeling phenomena seen in nature, to solving complex engineering problems that exist in the world.
There exists a subset of algorithms within the field of evolutionary computation that focus on solving optimization problems --- evolutionary algorithms.

Evolutionary algorithms are probabilistic search algorithms where evolutionary processes are used sample the space of possible solutions.
At any point in time, the set of candidate solutions under consideration is regarded as the population.
Each solution in the population is evaluated based on a given optimization problem to determine the set of solutions to act as parents for the construction of a new generation of solutions.
Offspring produced from the set of parent solutions will be subject to a source of variation, typically either mutations to their underlying representation or recombination with other parent solutions.

The previous description makes it clear that decisions regarding a combination of criteria, parameters, and procedures must be determined before an evolutionary algorithm can be executed.
Some of these decisions include determining a solutions' underlying representation, mutation operators, selection scheme, stopping criteria, etc.
Having to describe every criteria, parameter, and procedure can make it difficult to understand and compare different evolutionary algorithms.
**This work focuses on mitigating this issue by presenting a conceptual framework to better describe selection schemes.**

More information can be found at this [link](https://github.com/jgh9094/Selection-Scheme-Diagnotics-Part-I).

---
### <a name="ssd">Selection Scheme Diagnostics</a>

Evolutionary algorithms are a great set of tools to use when it is not possible to represent the optimization problem in a clean mathematical formula and no assumptions about the fitness landscape are known.
The optimization problems that evolutionary algorithms attempt to solve possess characteristics that are common across different optimization problems; where these characteristics are captured and represented by a set of diagnostics.
Unfortunately, there is no way to guarantee that an evolutionary algorithm can produce an optimal solution for a given optimization problem.
This can happen due to the complex nature of the optimization problem or an evolutionary algorithms design does not allow it to.

An evolutionary algorithm has a number of working components when attempting to solve an optimization problem, and each component has an impact on whether or not optimal solution being discovered.
This can make it difficult to understand the impact of each component has on an evolutionary algorithms’ performance.
In this work, the selection scheme is isolated to better understand its strengths and weaknesses.

Each selection scheme of interest is evaluated against the set of diagnostics, where the set of diagnostics may change as new optimization problem characteristics are discovered.
This in turn gives us a *profile* for each selection scheme, where a profile presents information to the reader about the kinds of optimization problems a selections scheme will perform well against.
It can be difficult to build the optimal evolutionary algorithm for a given optimization problem, but these profiles can give better insight to the

More information can be found at this [link](https://github.com/jgh9094/Selection-Scheme-Diagnotics-Part-I).
