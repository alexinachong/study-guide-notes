# Web


## REST (W1D1)
Representational State Transfer: a set of design principles (not specific to the web) for making network communication more scalable and flexible. REST is *not* a protocol since it does not prescribe implementation details.

The Fielding Constraints are architectural constraints that a system must satisfy to be considered RESTful.

### What are the three primary Fielding constraints?
1. **Client-Server**
   The network must be made up of clients and servers.

   *Client*: A computer that wants to interact with the resources stored on the server.
   *Server*: A computer that has resources of interest.
2. **Stateless**
   Each request is standalone, and servers and clients do not need to keep track of each other's state (or existence, once the request is complete).
3. **Uniform Interface**
   Ensures that there is a common language between servers and clients that allows each part to be swapped out or modified without breaking the entire system.

   Achieved through 4 sub-constraints (see below)

### What sub-constraints make up a Uniform Interface?
1. Identification of Resources
2. Manipulation of Resources through Representations
3. Self-Descriptive Messages
4. Hypermedia

### Walk through an arbitrary example of a RESTful request/response cycle, and describe what makes it RESTful.
