# Error
http://racksburg.com/choosing-an-http-status-code/
http://stackoverflow.com/questions/942951/rest-api-error-return-good-practices
http://www.codingpedia.org/ama/error-handling-in-rest-api-with-jersey/
http://archive.oreilly.com/pub/post/restful_error_handling.html

# EBooks
https://apigee.com/about/resources/ebooks

![1](http://blog.cloud-elements.com/hs-fs/hubfs/Screen-Shot-2015-05-26-at-9.35.55-AM.png?t=1490379020301&width=506&name=Screen-Shot-2015-05-26-at-9.35.55-AM.png)
![1](http://blog.cloud-elements.com/hs-fs/hubfs/Screen-Shot-2015-05-26-at-9.36.04-AM-1.png?t=1490379020301&width=507&name=Screen-Shot-2015-05-26-at-9.36.04-AM-1.png)
![1](http://blog.cloud-elements.com/hs-fs/hubfs/Screen-Shot-2015-05-26-at-9.36.25-AM.png?t=1490379020301&width=506&name=Screen-Shot-2015-05-26-at-9.36.25-AM.png)
![1](https://d38wlcdzwz02m5.cloudfront.net/about/cdn/farfuture/Se8EqbxAePYS_hvM3Q1Cow_3CPIt7KASmJ866RoP4Ho/mtime:1440078969/sites/mktg-new/files/blog/Prag_REST_errors_1.png)
![1](https://d38wlcdzwz02m5.cloudfront.net/about/cdn/farfuture/ADeLlqsTIygJxr-lb_GA-JBCR7JFbUKikea16odGVn8/mtime:1440079021/sites/mktg-new/files/blog/Prag_REST_errors_2a.png)



![1](http://blogs.ca.com/wp-content/uploads/2017/01/API-Infinity-diagram-for-David-Chiu-blog-1024x576.jpg)

* [Web API Design](https://pages.apigee.com/rs/apigee/images/api-design-ebook-2012-03.pdf)
* [APIs For Dummies Apigee Special Edition](http://developer.pearson.com/sites/default/files/apigee-APIs-for-Dummies-eBook-2016-01.pdf)
* [APIs For Dummies IBM Special Edition](ftp://public.dhe.ibm.com/software/uk/pdf/api-service/WSM14025USEN.pdf)
* [REST CookBook](http://restcookbook.com/)

https://theamiableapi.com/2012/01/16/java-api-design-checklist/

http://geekswithblogs.net/JoshReuben/archive/2016/12/15/docker-rest-api-quickref.aspx
http://nordicapis.com/legos-api-strategy-resourcing-developers-building-business-case/

API Management and Resources

https://www.mulesoft.com/resources/api-management


# API Management 
* **Documentation** – Sounds boring, right? Still, one of the most common problems of developers is figuring out how an API works. Development time is too precious to waste in trial and error of an undocumented API. An API management service has to provide an easy way to read the documentation and enable developers to “try before they buy”. In some cases it is even possible to provide interactive documentation. Simplicity and usability are the keys!
* **Analytics and Statistics** – It is critical to understand how people use your API and get insights for your business.
* **Deployment** – Should be flexible and support public or private clouds, on-premises implementations, or combinations.
* **Developer engagement** – Engaging with your API consumers, developer or partners is important. Getting an easily accessible developer portal will significantly facilitate onboarding.
* **Sandbox environment** – This feature will increase both the value of an API and its adoption rate. What better than being able to develop and test your code.
* **Traffic management and caching** abilities.
* **Security** – APIs carry sensitive data, so it is important to protect the exposed information. The service has to at least provide  **identity and access management** for users and developers.
* **Monetization**– Provide the capability to monetize your API.
* **Availability** – Should be available, scalable and redundant. An API environment can become demanding and the service should be able to deal with any kind of errors, problems or temporary traffic spikes.
* **Support of Legacy systems**.


** To Proxy or not to Proxy?**

The vendors in the API management space provide a number of solutions across the above main categories but that does not mean they support everything. They are implementing their solution in three different ways: **Proxies, Agents or Hybrid**.

* API service providers that use the concept of a **Proxy**. Their solution “sits” between the customer and their users and the traffic goes through them. Proxies provide caching capabilities and protection of customer’s back-end infrastructure from traffic spikes. The main criticism they receive is that they increase the cost and bring up privacy and latency issues. Apigee, Mashape and Mashery are examples of such implementations.
* API service providers that use the concept of **agents**. Agents are plugins that integrate with your server. They do not get in the way of the API calls like proxies. As a result they do not introduce network latencies or 3rd-party dependencies. On the other side, features like caching are not easy to implement. 3scale is an example of such implementation.
* API service providers that use a **hybrid** approach. This means you may get an agent and a proxy. For example you may want to use a proxy for the caching and the agent for authentication. Companies like Apigee or 3scale we talked before are also moving to hybrid solutions.

# API Design Guidelines
* [WSO2 Rest API Design Guidelines](http://wso2.com/whitepapers/wso2-rest-apis-design-guidelines/)



# API Deployment
# API Access Control
# API Version

# API Checklist
https://zalando.github.io/restful-api-guidelines
https://pages.apigee.com/rs/351-WXY-166/images/API-54308-ProductBrief_Checklist_V4%20(1).pdf
http://www.kennethlange.com/posts/The-Ultimate-Checklist-for-REST-APIs.html
https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md
https://github.com/WhiteHouse/api-standards


# Tools
* [API Discovery Tools](https://blog.blendo.co/8-api-discovery-tools/)
* [API Discovery: 11+ Ways to Find APIs](http://nordicapis.com/api-discovery-11-ways-to-find-apis/)
* [10 Continuous Integration Tools to Spur API Development](http://nordicapis.com/10-continuous-integration-tools-spur-api-development/)
* [Tips and Tools for Debugging APIs](http://nordicapis.com/tips-and-tools-for-debugging-apis/)
* [API Management tools](https://www.developereconomics.com/api-management-tools-how-to-find-the-one-for-you)
https://restful.io/a-review-of-all-most-common-api-editors-6a720dc4f4e6#

# API Documentation
* [Ultimate Guide to 30+ API Documentation Solutions](http://nordicapis.com/ultimate-guide-to-30-api-documentation-solutions/)
* [The Easiest Ways to Generate API Documentation](http://nordicapis.com/the-easiest-ways-to-generate-api-documentation/)
* [What is the Difference Between API Documentation, Specification, and Definition?](http://nordicapis.com/difference-api-documentation-specification-definition/)

# API Design
* [Designing APIs for Humans](http://nordicapis.com/designing-apis-humans/)
* [API Design: Building and Enforcing an Internal Style Guide](http://nordicapis.com/api-design-building-and-enforcing-an-internal-style-guide/)
* [Decouple User Identity from API Design to Build Scalable Microservices](http://nordicapis.com/decouple-user-identity-from-api-design-to-build-scalable-microservices/)

# API Discovery & Assembly

# API Gateway
http://microservices.io/patterns/apigateway.html

# API Testing
* [9 Common Errors Made During API Testing](http://nordicapis.com/9-common-errors-made-during-api-testing/)

# API Lifecycle Mgmt & Governance
* [API Lifecycle Operations Stage: Marketing Your API](http://nordicapis.com/api-lifecycle-operations-stage-marketing-your-api/)
* [API Lifecycle Development Stage: Deploying Your API](http://nordicapis.com/api-lifecycle-development/)
* [API Lifecycle Analysis Stage: Preparing Your Prelaunch API Strategy](http://nordicapis.com/api-lifecycle-analysis-stage-preparing-your-api-strategy-pre-launch/)
* [Envisioning The Entire API Lifecycle](http://nordicapis.com/envisioning-the-entire-api-lifecycle/)

# API Management service 

# API Security
* [API Security: The 4 Defenses of The API Stronghold](http://nordicapis.com/api-security-the-4-defenses-of-the-api-stronghold/)
* [Maintaining API Security in a Continuous Delivery Environment](http://nordicapis.com/maintaining-api-security-in-a-continuous-delivery-environment/)
* [Techniques and Technologies to Increase API Security](http://nordicapis.com/building-a-secure-api/)

# API Monetization
* [How to Grow and Profit Using a Freemium API Monetization Model](http://nordicapis.com/how-to-grow-and-profit-using-a-freemium-api-monetization-model/)
* [Top 5 API Monetization Models](http://nordicapis.com/top-5-api-monetization-models/)

# API Monitor
* [Monitor the Status of APIs with These 4 Tools](http://nordicapis.com/monitor-the-status-of-apis-with-these-4-tools/)

# API Analytics

# API Management

# Traffic control & mediation
# Workload optimization

# Community & Subscription management

# Lifecycle Mgmt & Governance

# API Designer

# Micro Gateway:

# URL

* [6 Techniques for 99.999% Uptime](http://nordicapis.com/6-techniques-99-999-uptime/)
* [The Core Principles of API Management](http://nordicapis.com/core-principles-api-management/)
* [Day in the Life of an API Developer Evangelist](http://nordicapis.com/day-in-the-life-of-an-api-developer-evangelist/)
* [API Gateways to Direct Microservices Architecture](http://nordicapis.com/api-gateways-direct-microservices-architecture/)
* [Token Design for a Better API Architecture](http://nordicapis.com/token-design-better-api-architecture/)
* [8 Keys To Creating A Truly Usable API](http://nordicapis.com/8-keys-to-creating-a-truly-usable-api/)
* [Designing Evolvable APIs for the Web: Formats](http://nordicapis.com/designing-evolvable-apis-for-the-web-formats/)
* [Description-Agnostic API Development with API Transformer](http://nordicapis.com/optimizing-apis-for-mobile-apps/)
* [Architecting an API Backend](http://nordicapis.com/architecting-an-api-backend/)
* [Beautiful UI Design for API Developer Portals](http://nordicapis.com/beautiful-ui-design-for-api-developer-portals/)
* [5 Benefits of Using Virtualization to Test Your API](http://nordicapis.com/5-benefits-of-using-virtualization-to-test-your-api/)
* [How To Control User Identity Within Microservices](http://nordicapis.com/how-to-control-user-identity-within-microservices/)
* [7 Important API Design Lessons](http://nordicapis.com/7-api-design-lessons-world-tour-roundup/)
* [Equipping Your API With The Right Armor](http://nordicapis.com/api-security-equipping-your-api-with-the-right-armor/)
* [Success vs. Failure – The Importance of API Metrics](http://nordicapis.com/success-vs-failure-the-importance-of-api-metrics/)
* [API Platform Defined: When an API Provider is a Platform](http://nordicapis.com/api-platform-defined-api-provider-is-a-platform/)
* [Why API Developer Experience Matters More Than Ever](http://nordicapis.com/why-api-developer-experience-matters-more-than-ever/)
* [Marketing your Public API](http://nordicapis.com/marketing-your-public-api/)


# API Policy Management 
* [Policy Management for APIs, Services, and Apps](http://blog.cobia.net/cobiacomm/2013/04/09/policy-management-for-apis-services-and-apps/)
* [Policy reference overview](http://docs.apigee.com/api-services/reference/reference-overview-policy)

# API Policy Enforcement


![1](http://b.content.wso2.com/sites/all/product-pages/images/apim-overview.png)
