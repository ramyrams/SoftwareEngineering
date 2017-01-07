# Features


## Design and Prototype APIs
* Design APIs, gather developers' feedback before implementing (API First Design). Design can be done from the publishing interface or via importing an existing Swagger 2.0 definition
* Deploy a prototyped API, provide early access to APIs, and get early feedback
* Mock API implementation using JavaScript
* Supports publishing SOAP, REST, JSON, and XML style services as APIs
* Pre-loaded sample APIs for a hassle-free first experience

## Publish APIs and Govern API Use
Publish APIs to external consumers and partners, as well as to internal users
Ability to publish APIs to a selected set of gateways in a multi-gateway environment
Support enforcement of corporate policies for actions like API subscriptions, application creation, etc. via customizable workflows
Manage API visibility and restrict access to specific partners or customers
Manage API lifecycle from cradle to grave: create, publish, block, deprecate, and retire
Publish both production and sandbox keys for APIs to enable easy developer testing
Manage API versions and deployment status by version
One-click deployment to API gateway for immediate publishing
Customize the API lifecycle, including executing custom behavior on lifecycle transitions

## Control Access and Enforce Security
Restrict API access tokens to domains/IPs
Validate APIs payload contents against a schema
Apply security policies to APIs (authentication, authorization)
Rely on OAuth2 standard for API access (implicit, authorization code, client, SAML, IWA Grant Type)
Plug third-party key servers in lieu of the default one, for application registration, Oauth2 token generation & validation
Block a subscription and restrict a complete application
Associate API to system-defined service tiers
Generate JSON web tokens for consumption by back-end servers
Leverage XACML for entitlements management and fine-grain authorization
Configure Single Sign-On (SSO) using SAML 2.0 for easy integration with existing web apps
Threat protection, bot detection and token-fraud detection

##Developer Portal

Graphical experience similar to popular applications stores
Browse and search APIs by provider, tags, or name
Provision API keys
Subscribe to APIs and manage subscriptions on per-application basis
Subscriptions can be at different service tiers based on expected usage levels
Interactive API Test console
Internationalization support
Notifications enabled for new versions of subscribed APIs
Common view of the store for users registered under same organization

##Manage Developer Community

Self-registration for developer community to subscribe to APIs
Developer interaction with APIs via forums, comments, and ratings
View API consumer analytics
Tools for API product managers to proactively manage API subscriptions
Tooling to develop services, features and artifacts and manage their links and dependencies through a simplified graphical editor

##Manage and Scale API Traffic

API gateway can act as SSL termination point
Separate production and sandbox traffic on different API gateways
Supports protocol transformation, data transformation, and API composition
Maps between HTTP(s) and other protocols, such as JMS or writing to file systems
Traffic Manager enforces rate limiting and throttling dynamically based on usage quotas and bandwidth quotas
Protect API backends with a throttling hard limit
Horizontally scalable with easy deployment into cluster using proven routing infrastructure
Extremely high performance pass-through message routing with minimal latency
Supports up to 1300 TPS on a single node

## Monitor and Monetize

API usage published to pluggable analytics framework (requests, responses, faults, throttling, subscriptions, self-sign ups to name a few)
Out-of-the-box support for WSO2 Data Analytics Server and Google Analytics.
Provides statistical graphs such as API latency and API usage comparison that help monitor API and application performance
Ability to analyze logs pertaining to application errors, API deployment stats, login errors, no of API failures, access token errors
Live log viewer
Track consumer analytics per API, per API version, per tiers, and per consumer
Configurable payment schemes to monetize API usage
Monitor SLA compliance
Publish your own events and create your own dashboards

## Pluggable, Extensible, and Themeable

All components are highly customizable through styling, theming, and code extensions
Developer portal is implemented with JavaScript/CSS/HTML5 for easy customization and theming
Responsive design for Developer portal
All publishing/portal functionality is exposed via a REST API, which allows to create your own portal or automate API deployment through DevOps
Pluggable to third-party analytics systems and billing systems
Pluggable to existing user repositories including Microsoft Active Directory, LDAP, databases, or Apache Cassandra
Components usable separately: developer portal can be used to catalog APIs deployed in third-party gateways

## Easily Deployable in Your Enterprise

Role-based access control for managing users and their authorization levels
Developer portal can be deployed in DMZ for external access with publisher inside the firewall for private control
Different user stores for developer-focused portal and internal operations in publisher
Integrates with enterprise identity systems including LDAP and Microsoft Active Directory
Gateway can be deployed in DMZ with controlled access to WSO2 Identity Server (for authentication/authorization) and governance database behind firewall

## WSO2 Platform Multi-tenancy Support
* Run a single instance and provide API management to multiple customers, each in their own domain
Share APIs between different departments in a large enterprise
