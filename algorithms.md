# Algorithms

## Graphs (W1D1)

### How do we define a graph mathematically?

### What is the difference between directed, undirected, weighted, and unweighted?

### Give an example of various types of graphs (Weighted Undirected, Unweighted Directed, Unweighted Undirected, etc.)

### What makes a graph a simple graph? What attributes would make it not simple?

### What is the maximum number of edges in a directed simple graph? Undirected simple graph? Answer should be in terms of `N`.

### Describe the levels of connectivity a graph can have (strongly connected, weakly connected).

### What are cycles?

### What are some naive ways we can store and traverse graphs? Be able to discuss time/space complexity of these approaches, and what issues we may face.

## Graph Adjacency Matrix / List (W1D2)

### Give a high level overview of an Adjacency Matrix.

### If we were only concerned about time complexity, is an Adjacency Matrix efficient? Why/why not?

### If we were only concerned about space complexity, is an Adjacency Matrix efficient? Why/why not?

### Give a high level overview of an Adjacency List.

### What benefits do we get from an Adjacency List?


## Recursion (W2D1)

### What is a base case in recursion? Why do we need one? Do we always need one?
The base case is the smallest or simplest case that we could encounter in our problem. As we dive deeper and deeper into our call stack, the base case acts as a stopping point or limit for our function, so that our code will eventually return a result (to slingshot back up the call stack) and not enter an infinite loop. We always need a base case in our recursive functions to avoid a stack overflow error.

### What exactly is a Stack Overflow?

### Describe direct and indirect recursion.
