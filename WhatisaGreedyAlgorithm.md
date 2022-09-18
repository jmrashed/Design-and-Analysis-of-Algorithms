# What is a Greedy Algorithm?

In **Greedy Algorithm** a set of resources are recursively divided based on the maximum, immediate availability of that resource at any given stage of execution.

To solve a problem based on the greedy approach, there are two stages

1. Scanning the list of items
2. Optimization

These stages are covered parallelly in this Greedy algorithm tutorial, on course of division of the array.

To understand the greedy approach, you will need to have a working knowledge of recursion and context switching. This helps you to understand how to trace the code. You can define the greedy paradigm in terms of your own necessary and sufficient statements.

## History of Greedy Algorithms

Here is an important landmark of greedy algorithms:

- Greedy algorithms were conceptualized for many graph walk algorithms in the 1950s.
- Esdger Djikstra conceptualized the algorithm to generate minimal spanning trees. He aimed to shorten the span of routes within the Dutch capital, Amsterdam.
- In the same decade, Prim and Kruskal achieved optimization strategies that were based on minimizing path costs along weighed routes.
- In the ’70s, American researchers, Cormen, Rivest, and Stein proposed a recursive substructuring of greedy solutions in their classical introduction to algorithms book.
- The Greedy search paradigm was registered as a different type of optimization strategy in the NIST records in 2005.
- Till date, protocols that run the web, such as the open-shortest-path-first (OSPF) and many other network packet switching protocols use the greedy strategy to minimize time spent on a network.

## Greedy Strategies and Decisions

Logic in its easiest form was boiled down to “greedy” or “not greedy”. These statements were defined by the approach taken to advance in each algorithm stage.

For example, Djikstra’s algorithm utilized a stepwise greedy strategy identifying hosts on the Internet by calculating a cost function. The value returned by the cost function determined whether the next path is “greedy” or “non-greedy”.

In short, an algorithm ceases to be greedy if at any stage it takes a step that is not locally greedy. The Greedy problems halt with no further scope of greed.

## Characteristics of the Greedy Algorithm

The important characteristics of a Greedy algorithm are:

- There is an ordered list of resources, with costs or value attributions. These quantify constraints on a system.
- You will take the maximum quantity of resources in the time a constraint applies.
- For example, in an activity scheduling problem, the resource costs are in hours, and the activities need to be performed in serial order.
- Characteristics of the Greedy Algorithm

## Why use the Greedy Approach?

Here are the reasons for using the greedy approach:

- The greedy approach has a few tradeoffs, which may make it suitable for optimization.
- One prominent reason is to achieve the most feasible solution immediately. In the activity selection problem (Explained below), if more activities can be done before finishing the current activity, these activities can be performed within the same time.
- Another reason is to divide a problem recursively based on a condition, with no need to combine all the solutions.
- In the activity selection problem, the “recursive division” step is achieved by scanning a list of items only once and considering certain activities.

## How to Solve the activity selection problem

In the activity scheduling example, there is a “start” and “finish” time for every activity. Each Activity is indexed by a number for reference. There are two activity categories.

1. considered activity: is the Activity, which is the reference from which the ability to do more than one remaining Activity is analyzed.
2. remaining activities: activities at one or more indexes ahead of the considered activity.

The total duration gives the cost of performing the activity. That is (finish – start) gives us the durational as the cost of an activity.

You will learn that the greedy extent is the number of remaining activities you can perform in the time of a considered activity.

Architecture of the Greedy approach

### STEP 1)

Scan the list of activity costs, starting with index 0 as the considered Index.

### STEP 2)

When more activities can be finished by the time, the considered activity finishes, start searching for one or more remaining activities.

### STEP 3)

If there are no more remaining activities, the current remaining activity becomes the next considered activity. Repeat step 1 and step 2, with the new considered activity. If there are no remaining activities left, go to step 4.

### STEP 4 )

Return the union of considered indices. These are the activity indices that will be used to maximize throughput.
