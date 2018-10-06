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

   Achieved through 4 sub-constraints *(see below)*.

### What sub-constraints make up a Uniform Interface?
1. **Identification of Resources**  
   Each resource must be uniquely identified by a stable identifier (that is, one that does not change across interactions, nor when the state of the resource changes).

   If a resource gets moved to another identifier, the server should give the client a response indicating that the request was bad, and give it a link to the new location of the resource.
2. **Manipulation of Resources through Representations**  
   Client manipulates resources through sending representations to the server – usually a JSON object containing the content that it would like to add, delete, or modify.

   In REST, the server has full control of the resources, and is responsible for making any changes. When a client wishes to make changes to resources, it sends the server a representation of what it would like the resulting resource to look like. The server takes the request as a suggestion, but still has ultimate control.
3. **Self-Descriptive Messages**  
   A message that contains all the information that the recipient needs to understand it. There should not be additional information in a separate documentation or in another message.
4. **Hypermedia**  
   *Hypermedia*: Data sent from the server to the client that contains information about what the client can do next – in other words, what further requests it can make.

   In REST, servers should be sending only hypermedia (e.g., HTML) to clients.

### Walk through an arbitrary example of a RESTful request/response cycle, and describe what makes it RESTful.
A user enters a URL (UI: identification of resources) into their browser address bar. The client sends a GET request (UI: manipulation of resources through representations) to the server (client-server) to load that specific page (stateless). The server sends back a response containing a 200 OK HTTP status response code, the content-type, and the HTML (UI: hypermedia) for that page so the client knows how to interpret the message (UI: self-descriptive messages). 
