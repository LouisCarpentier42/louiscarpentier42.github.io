---
title: A heuristic algorithm using tree decompositions for the maximum happy vertices problem
authors:
  - first: Louis
    last: Carpentier
  - first: Jorik
    last: Jooken
  - first: Jan
    last: Goedgebeur
year: 2024
venue: Journal of Heuristics (JoH)
doi: 10.1007/s10732-023-09522-x
toc: true
---

Many problems are hard, _very hard_. This is not only for humans, but also for computers. Researchers have put significant effort into developing efficient algorithms for solving these hard problems. One such approach exploits a so-called tree decomposition to efficiently find solutions. However, this only works if the _treewidth_ of the tree decomposition is sufficiently small. This requirement cannot be guaranteed in practice. In this work, we created a heuristic algorithm using tree decompositions for the maximum happy vertices problem. Our algorithm finds good solutions (but not necessarily optimal) in only a fraction of the time, even if the treewidth is unbounded. 

On this page, I will explain what a tree decomposition is, how they are used to efficiently solve hard problems, and how we extended this approach to a heuristic algorithm. But first, how can we make a vertex happy?

## The Maximum Happy Vertices Problem

Before we can talk about happy vertices, we need to talk about graphs. A graph is a mathematical structure that is used to describe interconnected objects, for example people and their friends. Formally, a graph exists of vertices which represent the objects (e.g., people) and edges which connect the vertices (e.g., which persons are friends). These graphs are typically drawn as some connected circles, in which the circles are the vertices and their connections are the edges. Below figure shows an example of such graph. 

<figure>
    <img src="/assets/images/2024-joh/graph.png">
    <figcaption>An example of a graph with 8 vertices and 12 edges.</figcaption>
</figure>

The maximum happy vertices problem considers graphs in which the vertices are coloured, and we say that a vertex is _happy_ if it has the same colour as all its neighbours (i.e., the vertices it is connected to). For example, imagine you need to assign the seat arrangement on your wedding. The vertices could represent the invitees, the edges who are friends to each other, and the colour represents the table to which you assign the invitee. An invitee/vertex is happy if he sits together with many friends. Given a graph in which a small set of the vertices are coloured, the maximum happy vertices problem requires you to colour all the remaining vertices such that the number of happy vertices is maximised, such that the maximum number of invitees at your wedding is happy with their seat. An example is given below. 

<figure>
    <img src="/assets/images/2024-joh/mhv.png">
    <figcaption>An example of the maximum happy vertices problem. Given the graph above, in which vertex 2 is red and vertices 5 and 7 are green, we must colour the remaining vertices to maximise the number of happy vertices. If we colour vertices 1 to 4 in red, and the remaining vertices 5 to 8 in green, then there are 4 happy vertices (1, 2, 6 and 7) and 4 unhappy vertices (3, 4, 5 and 8).</figcaption>
</figure>

## The Tree Decompositions

What is a tree decomposition, but in layman terms 

+ Types of nodes in a tree decomposition

## Tree Decompositions to Efficiently Solve Hard Problems

How can you use tree decompositions for exact algorithms for the MHV problem

+ a note on the runtime complexity 

## Our Heuristic algorithm

What we do 
