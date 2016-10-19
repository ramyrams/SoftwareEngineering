https://i.ytimg.com/vi/15k-NZ4PMso/maxresdefault.jpg


Improving .NET Application Performance and Scalability - April 2004

# Fundamentals of Engineering for Performance

# Engineering for Performance
* Performance objectives enable you to know when your application meets your performance goals.
* Performance modeling provides a structured and repeatable approach to meeting your performance objectives.
* Architecture and design guidelines enable you to engineer for performance from an early stage.
* A performance and scalability frame enables you to organize and prioritize performance issues.
* Measuring lets you see whether your application is trending toward or away from the performance objectives.
* Providing clear role segmentation helps architects, developers, testers, and administrators understand their responsibilities within the application life cycle. Different parts of this guide map to the various stages of the product development life cycle and to the various roles.

![1](https://i-msdn.sec.s-msft.com/dynimg/IC7499.gif)
https://i-msdn.sec.s-msft.com/dynimg/IC104412.gif

Performance Categories
Category				Key Considerations
Coupling and cohesion	Loose coupling and high cohesion
Communication			Transport mechanism, boundaries, remote interface design, round trips, serialization, bandwidth
Concurrency				Transactions, locks, threading, queuing
Resource management		Allocating, creating, destroying, pooling
Caching					Per user, application-wide, data volatility
State management		Per user, application-wide, persistence, location
Data structures and algorithms	Choice of algorithm Arrays versus collections


![1](https://i-msdn.sec.s-msft.com/dynimg/IC7499.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC104412.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC31171.gif)

Life cycle mapping
* Gathering requirements. You start to define performance objectives, workflow, and key scenarios. You begin to consider workloads and estimated volumes for each scenario. You begin the performance modeling process at this stage by using early prototyping, if necessary.
* Design. Working within your architectural constraints, you start to generate specifications for the construction of code. Design decisions should be based on proven principles and patterns. Your design should be reviewed from a performance perspective. Measuring should continue throughout the life cycle, starting with the design phase.
* Development. Start reviewing your code early in the implementation phase to identify inefficient coding practices that could lead to performance bottlenecks. You can start to capture real metrics to validate the assumptions made in the design phase. Be careful to maintain a balanced approach during development; micro-optimization at an early stage is not likely to be helpful.
* Testing. Load and stress testing is used to generate metrics and to verify application behavior and performance under normal and peak load conditions.
* Deployment. During the deployment phase, you validate your model by using production metrics. You can validate workload estimates, resource utilization levels, response time, and throughput.
* Maintenance. You should continue to measure and monitor when your application is deployed in the production environment. Changes that may affect system performance include increased user loads, deployment of new applications on shared infrastructure, system software revisions, and updates to your application to provide enhanced or new functionality. Use your performance metrics to guide your capacity and scaling plans.





# Performance Modeling
![1](https://i-msdn.sec.s-msft.com/dynimg/IC153195.gif)

Why Model Performance?
What are the relevant code paths and how do they affect performance?
Where do the use of resources or computations affect performance?
Which are the most frequently executed code paths? This helps you identify where to spend time tuning.
What are the key steps that access resources and lead to contention?
Where is your code in relation to resources (local, remote)?
What tradeoffs have you made for performance?
Which components have relationships to other components or resources?
Where are your synchronous and asynchronous calls?
What is your I/O-bound work and what is your CPU-bound work?
What is the priority and achievability of different performance goals?
Where have your performance goals affected design?

https://i-msdn.sec.s-msft.com/dynimg/IC153195.gif


# Eight step performance model
1. Identify key scenarios. Identify scenarios where performance is important and scenarios that pose the most risk to your performance objectives.
2. Identify workload. Identify how many users and concurrent users your system needs to support.
3. Identify performance objectives. Define performance objectives for each of your key scenarios. Performance objectives reflect business requirements.
4. Identify budget. Identity your budget or constraints. This includes the maximum execution time in which an operation must be completed and resource utilization constraints, such as CPU, memory, disk I/O, and network I/O.
5. Identify processing steps. Break down your key scenarios into component processing steps.
6. Allocate budget. Spread your budget (determined in Step 4) across your processing steps (determined in Step 5) to meet your performance objectives (defined in Step 3).
7. Evaluate. Evaluate your design against objectives and budget. You may need to modify your design or spread your response time and resource utilization budget differently to meet your performance objectives.
8. Validate. Validate your model and estimates. This is an ongoing activity and includes prototyping, assessing, and measuring.

* [Read More](https://msdn.microsoft.com/en-us/library/ff647767.aspx)



# Design Guidelines for Application Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC109724.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC81061.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC73986.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC137901.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC167055.gif)

https://msdn.microsoft.com/en-us/library/ff647801.aspx


# Architecture and Design Review of a .NET Application for Performance and Scalability
https://msdn.microsoft.com/en-us/library/ff647792.aspx


![1](https://i-msdn.sec.s-msft.com/dynimg/IC41824.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC166271.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC99698.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC112166.gif)


#  Improving ASP.NET Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC25492.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC1883.gif)

https://msdn.microsoft.com/en-us/library/ff647790.aspx
https://msdn.microsoft.com/en-us/library/ff647787.aspx

# Improving Interop Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC121638.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC119876.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC132977.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC172270.gif)


# Improving Enterprise Services Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC86429.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC144884.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC133601.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC128727.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC93439.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC108845.gif)

https://msdn.microsoft.com/en-us/library/ff647809.aspx


# Improving Web Services Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC54087.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC104836.gif)
https://msdn.microsoft.com/en-us/library/ff647786.aspx


# Code Review: .NET Application Performance


#  Improving SQL Server Performance
https://i-msdn.sec.s-msft.com/dynimg/IC42074.gif

https://msdn.microsoft.com/en-us/library/ff647793.aspx


# Measuring .NET Application Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC31171.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC49462.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC142896.gif)

https://msdn.microsoft.com/en-us/library/ff647791.aspx


# Testing .NET Application Performance
![1](https://i-msdn.sec.s-msft.com/dynimg/IC161505.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC121186.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC21129.gif)
![1](https://i-msdn.sec.s-msft.com/dynimg/IC91535.gif)

https://msdn.microsoft.com/en-us/library/ff647788.aspx


Tuning .NET Application Performance
https://msdn.microsoft.com/en-us/library/ff647813.aspx
