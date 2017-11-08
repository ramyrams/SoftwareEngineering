High Availability 

Performance and scalability techniques 101
https://www.webforefront.com/performance/scaling101.html

Architecting for High Availability
https://www.slideshare.net/AmazonWebServices/architecting-for-high-availability
High Availability in 37 Easy Steps
https://www.slideshare.net/tserong/high-availability-in-37-easy-steps
High Availability (HA) Explained
https://www.slideshare.net/d0cent/high-availability-explained

https://www.slideshare.net/kamesh001/high-available-for-openstack

https://www.slideshare.net/akelios/high-availability-and-disaster-recovery

AWS re:Invent 2014/2016 | (SOV204) Scaling Up to Your First 10 Million Users
https://www.youtube.com/watch?v=n28lDDdlnVg
https://www.youtube.com/watch?v=ccojvcQq858

Design patterns and plan for developing high available azure applications
https://www.slideshare.net/himanshus_sahu/design-patterns-and-plan-for-developing-high-available-azure-applications

* Diagnostic phase—Diagnose the problem and determine an appropriate course of action.
* Procurement phase—Identify, locate, transport, and physically assemble replacement hardware, software, and backup media.
* Base Provisioning phase—Configure the system hardware and install a base OS.
* Restoration phase—Restore the entire system from media, including the system files and user data.
* Verification phase—Verify the functionality of the entire system and the integrity of user data.

https://www.design-reuse.com/articles/3671/design-patterns-for-high-availability.html


https://msdn.microsoft.com/en-us/magazine/dd727504.aspx

https://msdn.microsoft.com/en-us/library/cc750543.aspx


# High Availability Architecture
https://www.getfilecloud.com/supportdocs/download/attachments/8160924/Capture.JPG


https://softwareengineering.stackexchange.com/questions/338680/how-to-design-a-high-availability-application
Scallability

http://www.fromdev.com/2014/02/Scalability-Books-Web-Architects.html
https://www.keycdn.com/blog/scalability-testing/


https://techbeacon.com/web-performance-testing-top-12-free-open-source-tools-consider

https://www.keycdn.com/blog/network-bandwidth/

https://www.keycdn.com/blog/speed-index/

https://www.keycdn.com/blog/website-architecture/


https://www.keycdn.com/blog/website-performance-metrics/


https://www.keycdn.com/blog/web-application-security-best-practices/
https://www.keycdn.com/blog/cdn-cache/
https://www.keycdn.com/blog/cdn-traffic-to-your-website/
https://www.keycdn.com/blog/web-performance-advice/
https://www.keycdn.com/blog/https-performance-overhead/
https://www.keycdn.com/blog/web-performance-experts/
https://www.keycdn.com/blog/scale-website-traffic/
https://www.keycdn.com/blog/http-to-https/
https://www.keycdn.com/blog/cdn-performance/
https://www.keycdn.com/blog/cors-cdn/

https://www.keycdn.com/blog/expire-header-and-cache-control/
https://www.keycdn.com/blog/live-streaming-rtmp-and-hls/
https://www.keycdn.com/blog/analyze-cdn-raw-logs-in-real-time/
https://blogs.msdn.microsoft.com/sql_pfe_blog/2013/06/15/an-overview-of-high-availability-and-disaster-recovery-solutions-available-for-sql-server/
https://www.keycdn.com/blog/cdn-analytics/
https://www.keycdn.com/blog/parallel-downloads-across-domains/
https://www.keycdn.com/blog/quic/
https://www.keycdn.com/blog/a-slow-website-time-to-first-byte-ttfb/
https://www.keycdn.com/blog/http-cache-headers/
https://www.keycdn.com/blog/how-to-optimize-and-compress-image-files/
https://www.keycdn.com/blog/responsive-images/
https://www.keycdn.com/blog/why-use-a-cdn/
https://www.keycdn.com/blog/resource-hints/
https://www.keycdn.com/blog/browser-compatibility-testing-tools/
https://www.keycdn.com/blog/fastest-cdn/
https://www.keycdn.com/blog/optimize-images-for-web/
https://techbeacon.com/web-performance-testing-top-12-free-open-source-tools-consider
https://www.keycdn.com/blog/javascript-performance/
https://msdn.microsoft.com/en-us/library/ff647681.aspx
Scalability checklist
https://docs.microsoft.com/en-us/azure/architecture/checklist/scalability

Resiliency checklist
https://docs.microsoft.com/en-us/azure/architecture/checklist/resiliency


DevOps Checklist
https://docs.microsoft.com/en-us/azure/architecture/checklist/dev-ops


Availability checklist
https://docs.microsoft.com/en-us/azure/architecture/checklist/availability






A few ideas to think about:

Make sure your web app is stateless (no data are kept in memory or disk on the web server)
Scale out your web application into a load balanced cluster/set of at least 3 nodes (check out nginx)
Test your application in the load balanced setup to make sure the behaviour hasn't changed/affected by the new infrastructure changes. (Should be fine if you fixed #1)
Scale out the database into a cluster of at least 3 nodes
Make sure you have a good setup for monitoring and alerts of any failure.
Chaos testing: take down web nodes or database nodes randomly and see how the system reacts and if any impact on availability and how to improve.



Like most complex subjects scalability defies easy and meaningful categorization. Some points I find common are:

0. Optimize browser code. A fast loading site makes for a good user experience.
1. Move work to the browser. Put as much of the UI logic in the browser as possible to offload the server, keep the user experience crisp. 
2. Use Ajax to make targeted requests and keep up with events.
3. Cache content close to the edge. Use a CDN (when you can) to serve static content as close to the browser as possible because this makes a better user experience.
4. Thin, load balanced, web servers. Implement functionality by load balancing requests across backend servers. Use a scripting language like Ruby, PHP, Python etc to compose pages. Scale by adding more machines.
5. Reverse proxy caching. Don't hit the backend unless you need to.
6. Connect to the backend using a service layer interface. Web server scripting code doesn't implement (much) business logic. It should glue together information gathered from encapsulated services that implement the business logic. Scale by asynchronously queuing requests and load balancing them across more servers.
7. Cache application level objects. Shed load from the database by putting a cache between the service layer and the database. Avoid disk and work from RAM as much as possible. This doesn't just mean do what you did before, just with cache, it means actively develop around the idea that you have fast in memory access available.
8. Shard. Make it so work can be parallelized to the degree you need to scale.
9. Share nothing. Parallelizing work means minimizing sharing and dependencies between components.
10. Cloud yourself. Make an elastic architecture that can grow and shrink horizontally.
11. Use *aaS. Use a storage service, a CPU service, and whatever else you can as a service. Do as little as you can get away with so you can spend time on your own application. Leverage economies of scale in areas that don't need to be your core competency.
12. Automate. Don't deploy by hand or do anything you can convince a machine to do for you.
13. Monitor. Monitor everything all the time and use that information to make your system better.
14. Use appropriate database technology. This is of course the tricky part and obviously interacts with all the other choices that have been made. With all the other strategies in place it's quite possible you can get away with a relatively simple database setup. Caching layers can protect the database from load and avoid complex queries and other database killers. Or maybe use web scale databases like BigTable or SimpleDB.

So far I've identified these:

- Hardware scalability:
- scale out
- scale up

- Cache
What types of cache are there? app-level, os-level, network-level, I/O-level?
- Load Balancing
- DB Clustering

