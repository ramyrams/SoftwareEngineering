Objects and Values
Classes and Interfaces
Method Design Principles
Modeling and Inheritance
Implementing Inheritance
Design by Contract
Role Objects
Collaboration-based Design
Design Patterns
Object Creation
Singleton Objects
Domain-Driven Design
Framework Design
Error and Exception Handling
Meta-Object Protocols

# Catalogs

* **Patterns of Enterprise Application Architecture**	Concentrates on Enterprise Application Architecture in the context of a layered architecture. Main sections cover domain logic, web presentations, database interaction, offline concurrency (by David Rice) and distribution. Database interaction is the largest section with many patterns on object-relational mapping issues.
* **Core J2EE Patterns**	Enterprise Application Architecture patterns in the context of the Java J2EE platform. Although the patterns are focused around the J2EE platform, the patterns are usually equally applicable (albeit with a twist) to other enterprise application platforms.
* **Enterprise Integration Patterns**	I've increasingly come to the view that integration through asynchronous messaging is one of the most effective ways to integrate disparate enterprise applications. EIP is a foundation collection of patterns for this approach.
* **Microsoft Enterprise Solution Patterns**	Microsoft's first collection of enterprise software patterns. Sections include patterns on Web Presentation, Deployment, and Distributed Systems.
* **Microsoft Data Patterns**	A collection of patterns on data movement: replication and synchronization.
* Microsoft Integration Patterns	Microsoft's take on integration patterns. Sections cover strategies for an integration layer, approaches to system connections, and topologies for integration.
* **Domain Driven Design**	Building an object-oriented Domain Model is a popular approach to organizing domain logic. It works particularly well with complex domains. It's downside is that it is difficult to do well. These patterns describe how to think about building and structuring a rich domain model, as well as how to recognize and overcome the real-world obstacles that too-often prevent people from employing the modeling principles they know.
* **Analysis Patterns** See enough domain models, and you see certain kinds of structures repeatedly. This book was my attempt to capture these commonalities in the form of patterns. In lots of ways it's very much in need of an update, but the basic ideas are still pretty sound. If find this material useful, do make sure you look at the newer supplementary material that I put on my website.
* **Data Model Patterns**	Common patterns in data models. Since these are developed from a very conceptual approach, the patterns are useful for object modeling as well as data modeling.
* **Gang of Four**	The first, and most used, patterns book. These are mostly fundamental patterns which are not specifically for enterprise software development, but the enterprise patterns reference them widely.
* **POSA**	Particularly influential for its work on architectural patterns. Layers (for enterprise applications) and pipes and filters (for messaging) are foundations for much enterprise patterns work.


# Patterns
  * Gang of Four Patterns
  * Head First Patterns
  * Enterprise Patterns
  * Multi-Tier Patterns

  * Repository Pattern
  * Unit-of-Work Pattern
  * Active Record Pattern
  * CQRS Pattern

* Model View Controller
* Model View Presenter
* Model View ViewModel

# 23 Gang of Four (GoF) 
* Creational Patterns
  * Abstract Factory - Creates an instance of several families of classes
  * Builder - Separates object construction from its representation
  * Factory Method - Creates an instance of several derived classes
  * Prototype	 - A fully initialized instance to be copied or cloned
  * Singleton	- A class of which only a single instance can exist

* Structural Patterns
  * Adapter	- Match interfaces of different classes
  * Bridge	- Separates an object’s interface from its implementation
  * Composite	- A tree structure of simple and composite objects
  * Decorator	- Add responsibilities to objects dynamically
  * Facade - A single class that represents an entire subsystem
  * Flyweight	- A fine-grained instance used for efficient sharing
  * Proxy	- An object representing another object

* Behavioral Patterns
  * Chain of Resp. - A way of passing a request between a chain of objects
  * Command - Encapsulate a command request as an object
  * Interpreter -	A way to include language elements in a program
  * Iterator - Sequentially access the elements of a collection
  * Mediator - Defines simplified communication between classes
  * Memento - Capture and restore an object's internal state
  * Observer - A way of notifying change to a number of classes
  * State	- Alter an object's behavior when its state changes
  * Strategy - Encapsulates an algorithm inside a class
  * Template Method - Defer the exact steps of an algorithm to a subclass
  * Visitor - Defines a new operation to a class without change



# Concurrency Patterns
* Active Object: Decouples method execution from method invocation that reside in their own thread of control. The goal is to introduce concurrency, by using asynchronous method invocation and a scheduler for handling requests.
* Balking: Only execute an action on an object when the object is in a particular state.
* Binding Properties: Combining multiple observers to force properties in different objects to be synchronized or coordinated in some way.
* Messaging pattern: The messaging design pattern (MDP) allows the interchange of information (i.e. messages) between components and applications.
* Double-checked locking: Reduce the overhead of acquiring a lock by first testing the locking criterion (the 'lock hint') in an unsafe manner; only if that succeeds does the actual lock proceed. Can be unsafe when implemented in some language/hardware combinations. It can therefore sometimes be considered an anti-pattern.
* Event-based asynchronous: Addresses problems with the Asynchronous pattern that occur in multithreaded programs.[10]
* Guarded suspension: Manages operations that require both a lock to be acquired and a precondition to be satisfied before the operation can be executed.
* Lock: One thread puts a "lock" on a resource, preventing other threads from accessing or modifying it.[11][7]
* Monitor object: An object whose methods are subject to mutual exclusion, thus preventing multiple objects from erroneously trying to use it at the same time.
* Reactor: A reactor object provides an asynchronous interface to resources that must be handled synchronously.
* Read-write lock: Allows concurrent read access to an object but requires exclusive access for write operations.
Scheduler: Explicitly control when threads may execute single-threaded code.
* Thread pool: A number of threads are created to perform a number of tasks, which are usually organized in a queue. Typically, there are many more tasks than threads. Can be considered a special case of the object pool pattern.
* Thread-specific storage: Static or "global" memory local to a thread.

# Data Access Patterns
* ORM Patterns: Domain Object Factory, Object/Relational Map, Update Factory
* Resource Management Patterns: Resource Pool, Resource Timer, Retryer, Paging Iterator
* Cache Patterns: Cache Accessor, Demand Cache, Primed Cache, Cache Collector, Cache Replicator
* Concurrency Patterns: Transaction, Optimistic Lock, Pessimistic Lock


# Enterprise Patterns
* Presentation Tier Patterns: Intercepting Filter, Front Controller, View Helper, Composite View, Service to Worker, Dispatcher View
* Business Tier Patterns: Business Delegate, Value Object, Session Facade, Composite Entity, Value Object Assembler, Value List Handler, Service Locator
* Integration Tier Patterns: Data Access Object, Service Activator


* Real-Time Patterns
* Architecture Patterns: Layered Pattern, Channel Architecture Pattern, Component-Based Architecture, Recursive Containment Pattern and Hierarchical Control Pattern, Microkernel Architecture Pattern, Virtual Machine Pattern
* Concurrency Patterns: Message Queuing Pattern, Interrupt Pattern, Guarded Call Pattern, Rendezvous Pattern, Cyclic Executive Pattern, Round Robin Pattern
* Memory Patterns: Static Allocation Pattern, Pool Allocation Pattern, Fixed Sized Buffer Pattern, Smart Pointer Pattern, Garbage Collection Pattern, Garbage Compactor Pattern
* Resource Patterns: Critical Section Pattern, Priority Inheritance Pattern, Priority Ceiling Pattern, Simultaneous Locking Pattern, Ordered Locking Pattern
* Distribution Patterns: Shared Memory Pattern, Remote Method Call Pattern, Observer Pattern, Data Bus Pattern, Proxy Pattern, Broker Pattern
* Safety and Reliability Patterns: Monitor-Actuator Pattern, Sanity Check Pattern, Watchdog Pattern, Safety Executive Pattern, Protected Single Channel Pattern, Homogeneous Redundancy Pattern, Triple Modular Redundancy Pattern, Heterogeneous Redundancy Pattern



# Enterprise Application Architecture (P of EAA)
* Domain Logic Patterns: Transaction Script, Domain Model, Table Module, Service Layer
* Data Source Architectural Patterns: Table Data Gateway, Row Data Gateway, Active Record, Data Mapper
* Object-Relational Behavioral Patterns: Unit of Work, Identity Map, Lazy Load
* Object-Relational Structural Patterns: Identity Field, Foreign Key Mapping, Association Table Mapping, Dependent Mapping, Embedded Value, Serialized LOB, Single Table Inheritance , Class Table * Inheritance , Concrete Table Inheritance, Inheritance Mappers .
* Object-Relational Metadata Mapping Patterns: Metadata Mapping , Query Object, Repository.
* Web Presentation Patterns: Model View Controller, Page Controller , Front Controller, Template View  Transform View, Two-Step View , Application Controller 
* Distribution Patterns: Remote Facade , Data Transfer Object 
* Offline Concurrency Patterns: Optimistic Offline Lock , Pessimistic Offline Lock , Coarse Grained Lock, Implicit Lock
* Session State Patterns: Client Session State , Server Session State, Database Session State 
* Base Patterns: Gateway , Mapper , Layer Supertype , Separated Interface, Registry, Value Object , Money , Special Case , Plugin , Service Stub (504), Record Set


# Git Hub
* [Head First Design Patterns](https://github.com/bethrobson/Head-First-Design-Patterns)

https://en.wikipedia.org/wiki/Architectural_pattern
https://en.wikipedia.org/wiki/Interaction_design_pattern
https://en.wikipedia.org/wiki/Software_design_pattern



* [MVVM Pattern Cheat Sheet and Flow](http://www.alextells.com/wp-content/uploads/2014/08/9fc37cfa186c24407739ebcc3191e014.png)





![1](http://dirkriehle.com/wp-content/uploads/2016/01/design-space-table-1024x650.png)
![1](http://www.linuxidc.com/upload/2015_12/151203132216072.png)
![1](http://image.slidesharecdn.com/DesignPatterns-123478276166-phpapp03/95/design-patterns-69-728.jpg)
![1](http://www.demiliani.com/immaginiblog/patterns/patterns2.jpg)
![1](http://vis.berkeley.edu/papers/infovis_design_patterns/pattern_map.gif)
![1](http://3.bp.blogspot.com/-39vWE8gscNg/UUTcMbVzRCI/AAAAAAAAAU4/ZbZJdWI-pZQ/s1600/Screen+Shot+2013-03-16+at+4.54.48+PM.png)
![1](http://coe.aceinfosolutions.com/sites/default/files/a%26e%20layers%20graphic.jpg)
![1](http://image.slidesharecdn.com/8dnenjjhq6iaqjxqfekm-signature-e311f9d5f5b8de7d3279f087d79ee0e2e6a76ff2f90cfca1d34f7dd81ce1bb15-poli-150219013320-conversion-gate01/95/case-study-integrating-azure-with-google-app-engine-10-638.jpg)
![1](http://asp.net/media/2578149/Windows-Live-Writer_8c4963ba1fa3_CE3B_Repository_pattern_diagram_1df790d3-bdf2-4c11-9098-946ddd9cd884.png)
![1](https://media-www-asp.azureedge.net/media/44907/dependency-injection-golf.png)
![1](https://i.ytimg.com/vi/BsuhLJb6vo0/maxresdefault.jpg)
![1](https://i.ytimg.com/vi/3-ycjbJkqv4/maxresdefault.jpg)
![1](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/8a67c0/easy-and-tricky-to-understand-the-factory-design-pattern-wit/Images/cms.png)
![1](https://i.ytimg.com/vi/bBcrJ_ivwnE/maxresdefault.jpg)
![1](https://i.ytimg.com/vi/cvqyJvVjxj4/maxresdefault.jpg)


