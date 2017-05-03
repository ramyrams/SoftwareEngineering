The Ins and Outs of Token Based Authentication
https://scotch.io/tutorials/the-ins-and-outs-of-token-based-authentication

How Companies Should Secure Your Passwords
https://scotch.io/bar-talk/how-companies-should-secure-your-passwords

https://i.stack.imgur.com/snQSG.png


Introducing The Auth0 Data Playbook


Easy Node Authentication: Linking All Accounts Together
https://scotch.io/tutorials/easy-node-authentication-linking-all-accounts-together

Token Based Authentication Made Easy
https://auth0.com/learn/token-based-authentication-made-easy/


Progressive Profiling
https://auth0.com/docs/user-profile/progressive-profiling

Progressive Profiling
https://auth0.com/docs/user-profile/progressive-profiling

Anomaly Detection
https://auth0.com/docs/anomaly-detection

# JSON Web Tokens (JWT)
5 Easy Steps to Understanding JSON Web Tokens (JWT)
https://medium.com/vandium-software/5-easy-steps-to-understanding-json-web-tokens-jwt-1164c0adfcec

The Anatomy of a JSON Web Token
https://scotch.io/tutorials/the-anatomy-of-a-json-web-token

https://cdn-images-1.medium.com/max/1000/1*SSXUQJ1dWjiUrDoKaaiGLA.png

http://blog.apcelent.com/images/json-web-token-authentication-apcelent.png


# Authorization flow

Applications use the following flow for requesting tokens:

1. The application directs the user to the OAuth server. On the page that opens, the user can grant the application access to specific account data.
2. The user grants access to personal data, and the OAuth server redirects the user to the address indicated by the developer.
The token that is issued (or the code for obtaining it) is embedded in the redirect URL. If the user refused access or an error occurred, an error message is appended to the redirect URL.
3. The application includes the received token in a request to a Yandex service that supports OAuth.

https://cdn-images-1.medium.com/max/1000/1*SSXUQJ1dWjiUrDoKaaiGLA.png


# Token lifespan

The token lifespan is how long the token can be used for authorization. The maximum lifespan depends on the permissions selected during application registration:
## Perpetual token
* Never expires and can only be revoked by the user.
* During application registration, the lifespan is displayed as "indefinite".
## Renewable token
* Expires after several months, but is renewed each time this token is used for authorization.
* The minimum lifespan is displayed during application registration, such as “at least 1 year”.
## RLimited token
* Expires after the duration specified for the respective access permissions.
* If multiple permissions were selected during application registration, the shortest time limit is applied to the token. For example, permissions to access Yandex.Metrica are set to 1 year, while permissions for using Yandex.Post Office are set to 180 days. This means that a token with permissions for both Yandex.Metrica and Yandex.Post Office will be valid for no longer than 180 days.
## RRevoking a token
Users can revoke any OAuth tokens that have been issued for their accounts:
* To revoke all tokens that were ever issued for an account, the user can change the password or .
* To revoke tokens that were issued to a specific application, the user can deny access for this application on the .

# API Gateway OAuth 2.0
* [Complete Tutorial](https://docs.oracle.com/cd/E50612_01/doc.11122/oauth_guide/content/oauth_intro.html)

API Gateway OAuth 2.0 Authentication Flows
https://docs.oracle.com/cd/E50612_01/doc.11122/oauth_guide/content/oauth_flows.html


# What is Token based authentication
Token based authentication allow client application to access the restricted resources of a server side application. Token based authentication uses a bearer token between client and server to access the resources. And to get the token, client application first send a request to Authentication server endpoint with appropriate credential. If the username and password is found correct then the Authentication server send a token to client as a response and the client application then use the token to access the restricted resources in next requests. ASP.Net Web API uses OWIN OAuth middleware for Authentication server operations.

https://www.codeproject.com/KB/webservices/1090252/AuthServerFinal.jpg


# What is Cookie based authentication
https://www.codeproject.com/KB/webservices/1090252/CookiesFinal.jpg

Token based authentication vs Cookie based authentication

# Identy Server
Thirty Solution Patterns with the WSO2 Identity Server
https://medium.facilelogin.com/thirty-solution-patterns-with-the-wso2-identity-server-16f9fd0c0389

# identity-management
The Role of Identity and Access Management in the Era of Digital Transformation
https://medium.facilelogin.com/the-role-of-identity-and-access-management-in-the-era-of-digital-transformation-48a472ce3247

# Social Login

* Facebook
* Google+
* Twitter
* Yahoo!
* PayPal
* AOL
* LinkedIn

http://developers.janrain.com/wp-content/uploads/2015/12/Social-Login-Overview.png


1. User clicks login and chooses a social provider through which to authenticate. The Social Login widget supports both modal and embedded presentation modes.
2. User logs in on the selected identity provider’s site (for example, Facebook, Google+, Twitter, and so on) and approves the use of your application with their account. The Social Login widget supports both popup window and redirect-based login flows.
3. The social provider communicates with the Janrain servers and securely provides authentication and identity information. The type and amount of data provided depend on the provider being used. For more information, see User Data by Identity Provider.
4. Janrain posts an access token to your token URL.
5. Using the access token and your API key, your application can fetch data about the user through our Social Login REST API.
6. User data can be served to your site to customize the end-user experience.

# Identity Providers
http://developers.janrain.com/overview/social-login/identity-providers/identity-providers-2/


Health Care Idendity Provider
http://developers.janrain.com/overview/social-login/identity-providers/provider-setup/health-care-identity-providers/doccheck/

# Single Sign-On

Single Sign-On Overview

Single Sign-On with Social Login

Single Sign-On with Registration



Introducing AccessURL 2.0
https://medium.com/@jarredsumner/introducing-accessurl-2-0-103deb5e7d24


# TLS
Introducing TLS with Client Authentication
https://medium.com/cloudflare-blog/introducing-tls-with-client-authentication-59cede5151c1



How to encrypt your entire life in less than an hour
https://medium.freecodecamp.com/tor-signal-and-beyond-a-law-abiding-citizens-guide-to-privacy-1a593f2104c3

What’s your identity worth to you?
https://hackernoon.com/whats-your-identity-worth-to-you-4e8a302ed340

Hackers Stole My Website…And I Pulled Off A $30,000 Sting Operation To Get It Back
https://medium.freecodecamp.com/hackers-stole-my-website-and-i-pulled-off-a-30-000-sting-operation-to-get-it-back-143d43ee3742

