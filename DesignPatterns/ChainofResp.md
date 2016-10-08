Intent
Avoid coupling the sender of a request to its receiver by giving more than one object a chance to handle the request. Chain the receiving objects and pass the request along the chain until an object handles it.
Launch-and-leave requests with a single processing pipeline that contains many possible handlers.
An object-oriented linked list with recursive traversal.

Problem

There is a potentially variable number of "handler" or "processing element" or "node" objects, and a stream of requests that must be handled. Need to efficiently process the requests without hard-wiring handler relationships and precedence, or request-to-handler mappings.
https://sourcemaking.com/files/v2/content/patterns/Chain_of_responsibility1.svg

http://www.vincehuston.org/dp/chain.html
http://www.javaworld.com/article/2072857/java-web-development/the-chain-of-responsibility-pattern-s-pitfalls-and-improvements.html


# Check list
The base class maintains a "next" pointer.
Each derived class implements its contribution for handling the request.
If the request needs to be "passed on", then the derived class "calls back" to the base class, which delegates to the "next" pointer.
The client (or some third party) creates and links the chain (which may include a link from the last node to the root node).
The client "launches and leaves" each request with the root of the chain.
Recursive delegation produces the illusion of magic.

# Rules of thumb

Chain of Responsibility, Command, Mediator, and Observer, address how you can decouple senders and receivers, but with different trade-offs. Chain of Responsibility passes a sender request along a chain of potential receivers.
Chain of Responsibility can use Command to represent requests as objects.
Chain of Responsibility is often applied in conjunction with Composite. There, a component's parent can act as its successor.



# Code
https://www.tutorialspoint.com/design_pattern/chain_of_responsibility_pattern.htm
https://dzone.com/articles/design-patterns-uncovered-chain-of-responsibility

https://i.ytimg.com/vi/BsuhLJb6vo0/maxresdefault.jpg
https://i.ytimg.com/vi/Izh9x_VoNUg/maxresdefault.jpg
https://sourcemaking.com/files/v2/content/patterns/Chain_of_responsibility_1.svg
https://sourcemaking.com/files/sm/images/patterns/Chain_of_responsibility_example.png
