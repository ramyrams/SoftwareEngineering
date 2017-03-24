# Plan Your API
* Key questions to ask:
* Who is our target user for this API
* Which of our products/ services do we want them to be working with? 
* What are THEIR use cases for integrating with our API?
* What technologies will they be using to integrate with our API?
* What other services will they want our API to interact with?
* Understand WHY you are building an API
* List out the user FUNCTIONALITY of your API
* Understand what TYPE of API you are building
* Think LONG TERM… like 2-3 years down the road


API Design Tooling From RAML
http://apievangelist.com/2014/03/01/api-design-tooling-from-raml/


http://apievangelist.com/2014/02/27/api-design-tooling-from-api-blueprint/
API Design Tooling From API Blueprint


# API Design Tooling From Swagger
http://apievangelist.com/2014/02/25/api-design-tooling-from-swagger/

# API Metrics and Analytics

# APIs Console
http://apievangelist.com/2011/05/21/google-apis-console/

# APIs Discovery Service
http://apievangelist.com/2011/05/21/google-apis-discovery-service/


# APIs Explorer
http://apievangelist.com/2011/05/21/google-apis-explorer/


Resource Stack
http://apievangelist.com/2013/07/01/the-resource-stack/



)



![1](http://kinlane-productions.s3.amazonaws.com/api_evangelist_site/blog/ct3y_zqviaaggk5.jpg)


![1](https://s3.amazonaws.com/kinlane-productions/whitepapers/api-evangelist-api-design.pdf)


API Documentation Solutions
http://apievangelist.com/2016/09/16/a-look-at-the-state-of-api-documentation-solutions/

# API Style
http://apistylebook.com/

# API Management 

# API Design Guide
https://geemus.gitbooks.io/http-api-design/content/en/

Google API Design Guide - https://cloud.google.com/apis/design/
API Design Guides Collection http://design.apievangelist.com/tools/design-guides/

API Design
http://apievangelist.com/2014/06/30/api-design-white-paper/


# API Observability
A Checklist For API Observability - http://apievangelist.com/2017/02/28/a-checklist-for-api-observability/


# API Definitions
http://apievangelist.com/2016/08/05/diff-tooling-for-json-yaml-and-markdown-versions-of-api-definitions/

What Is APIs.json? And What Is Next For the API Discovery Format?
http://apievangelist.com/2016/02/25/what-is-apisjson-and-what-is-next-for-the-api-discovery-format/
http://apievangelist.com/2014/06/30/apisjson-api-property-types/

http://apis.io/
1080 APIs in database by 211 maintainers.

http://theapistack.com/


My Brain Dump On An API Definition Fueled Life Cycle
http://apievangelist.com/2015/02/23/my-brain-dump-on-an-api-definition-fueled-life-cycle/

The Essential Building Blocks For Integration, Automation, and Reciprocity
http://apievangelist.com/2016/02/15/the-essential-building-blocks-for-integration-automation-and-reciprocity/


What Exactly Is APIs.json?
http://apievangelist.com/2015/01/05/what-exactly-is-apisjson/


# API definition format
* **Swagger** - The vision behind Swagger was not to make a company or to get people to use our service, it was strictly to solve a workflow problem. Initially the goal was centered around documentation and client tooling, but quickly realized it was much bigger, and became about managing the overall lifecycle of APIs.
* **API Blueprint** - API Blueprint is all about simplicity, and allowing people to have a structured conversation around an API, with the people who are actually going to be using it. Apiary is the conduit for this conversation, allowing developers to easily create a mock interface from the blueprint, share with consumers, and iterate as necessary.
* **RAML** - The motivation behind RAML was about seeking one source of truth, and a basic representation of an API. We used Swagger and API Blueprint, but neither fully met our vision. RAML was born, and is in alignment with Mulesoft's design first approach, and gave them the ability to design an API in a format that allowed them to sit down with stakeholders in a webinar and get instant feedback—bringing the API to forefront, not the implementation.


# Planning Your API 
* Designing the Spec/API
* Designing Your Resources 
* Designing Your Methods 
* Authorization and Authentication 
* Documenting and Sharing Your API 


#Anatomy Of API Call Failure
* Is the API Online?
* Did the server receive the request?
* Was URL request successful?
* Did the request timeout?
* Was there a server error?
* Was JSON receive successfully?
* Was JSON malformed?
* Was there an unexpected response?
* Were we able to map to JSON successfully?
* Is the JSON valid?
* Does local model match server model?

![1](https://blogs.mulesoft.com/wp-content/uploads/2014/11/action_list.gif)


![1](https://blogs.mulesoft.com/wp-content/uploads/2014/11/soap_vs_rpc_rest.gif)

# API Building Blocks
* [Adding Two More Building Blocks For API Rate Limiting](http://apievangelist.com/2014/12/30/adding-two-more-building-blocks-for-api-rate-limiting/)
* [50 Building Blocks Of The API Economy](http://apievangelist.com/2014/04/03/50-building-blocks-of-the-api-economy/)
* [Common Building Blocks of Cloud APIs](http://apievangelist.com/2014/03/11/common-building-blocks-of-cloud-apis/)
* [Some Of The Common Building Blocks of Payment APIs](http://apievangelist.com/2014/03/05/some-of-the-common-building-blocks-of-payment-apis/)
* [Common Building Blocks Of API Design](http://apievangelist.com/2014/03/04/common-building-blocks-of-api-design/)
* [What Are The Common Building Blocks of API Integration?](http://apievangelist.com/2014/01/16/what-are-the-common-building-blocks-of-api-integration/)
* [Building Blocks Of API Deployment](http://apievangelist.com/2014/07/01/building-blocks-of-api-deployment/)
* [50 Building Blocks Of The API Economy](http://apievangelist.com/2014/04/03/50-building-blocks-of-the-api-economy/)
* [Some Of The Common Building Blocks of Payment APIs](http://apievangelist.com/2014/03/05/some-of-the-common-building-blocks-of-payment-apis/)
* [Common Building Blocks Of API Design](http://apievangelist.com/2014/03/04/common-building-blocks-of-api-design/)
* [Common Building Blocks of API Integration](http://apievangelist.com/2014/01/16/what-are-the-common-building-blocks-of-api-integration/)
* [API Management Building Blocks](http://management.apievangelist.com/building-blocks/)
* [Some Of The Common Building Blocks Of API Deprecation](http://apievangelist.com/2016/04/13/some-of-the-common-building-blocks-of-api-deprecation/)
* [Adding Four New Building Building Blocks Providing An API Management API Blueprint](http://apievangelist.com/2015/03/04/adding-four-new-building-building-blocks-providing-an-api-management-api-blueprint/)
* [Essential Building Blocks For Integration, Automation, and Reciprocity](http://apievangelist.com/2016/02/15/the-essential-building-blocks-for-integration-automation-and-reciprocity/)


# Lifecycle of an API [Full Video](http://wso2.com/library/webinars/2016/02/planning-your-api-journey-the-lifecycle-of-an-api/)
![1](https://image.slidesharecdn.com/planningyourapijourneythelifecycleofanapi-160224055627/95/planning-your-api-journey-the-lifecycle-of-an-api-5-638.jpg?cb=1456293472)
![1](https://image.slidesharecdn.com/planningyourapijourneythelifecycleofanapi-160224055627/95/planning-your-api-journey-the-lifecycle-of-an-api-10-638.jpg?cb=1456293472)
![1](https://image.slidesharecdn.com/planningyourapijourneythelifecycleofanapi-160224055627/95/planning-your-api-journey-the-lifecycle-of-an-api-11-638.jpg?cb=1456293472)


* Users - User a user, edit a user, retrieve username, retreive password, reset pasword, view profile, Message uer.
* Messages - Send a message, create a draft, send a draft, delete draft, get message, mark message as read, mark message as unlead, move message to fodler, delete message.
* Products - View product, review product, add product to cart, add to wishlist
* Cart - View cart, add product, chage quantity, delete product, checkout

# Choosing a Spec
* Choosing the best specification for your company’s needs will make building, maintaining, documenting and sharing your API easier. 
* Because Spec-Driven Development encourages the use of a well tested, standardized spec, it is highly recommended that you choose from RAML, Swagger, Mashery IO Docs, tripit slate or API Blueprint. 

* [Modeling Web APIs](http://modeling-languages.com/modeling-web-api-comparing/)
* [API Spec Comparison Tool](http://www.mikestowe.com/2014/12/api-spec-comparison-tool.php)

# Descriptive Error Formats
## JSON API
http://jsonapi.org/format/#errors
```json
{	
	"error":	{	
		"errors":	[{	
			"id":	"error1_firstName",	
			"code":	"XB500",	
			"status":	"400",	
			"title":	"User	first	name	cannot	be	empty",	
			"detail":	 "The	 first	 name	 field	 is	 required	 to	
			have	a	value",	
			"href":	"http://docs.domain.ext/users/post"	
		},
		{	
			"id":	"error2_lastName",	
			"code":	"XB501",	
			"status":	"400",	
			"title":	"User	last	name	cannot	be	empty",	
			"detail":	 "The	 last	 name	 field	 is	 required	 to	
			have	a	value",	
			"href":	"http://docs.domain.ext/users/post"	
		}]
	}	
}
```
## Google Errors
```json
{	
	"error":	{	
		"code":	400,	
		"message":	"The	user	was	missing	required	fields",
		"errors":	[{	
		"domain":	"global",	
		"reason":	"MissingParameter",	
		"message":	"User	first	name	cannot	be	empty",	
		"locationType":	"parameter",	
		"location":	"firstName",	
		"extendedHelp":	
		"http://docs.domain.ext/users/post"	
	},
	{	
		"domain":	"global",	
		"reason":	"MissingParameter",	
		"message":	"User	last	name	cannot	be	empty",	
		"locationType":	"parameter",	
		"location":	"lastName",	
		"extendedHelp":	
		"http://docs.domain.ext/users/post"	
		}]
	}	
}
```
## vnd.error
https://github.com/blongden/vnd.error
```json
{	
	"total":	2,	
	"_embedded":	{	
		"errors":	[	{	
			"message":	“User	first	name	cannot	be	empty",	
			"logref":	“XB500”,	
			"_links":	{	
				"help":	{	"href":	"http://docs.domain.ext/users/post"	}	
			}	
		},	
		{	
			"message":	“User	last	name	cannot	be	empty",	
			"logref":	“XB501”,	
			"_links":	{	
				"help":	{	"href":	"http://docs.domain.ext/users/post"	}	
			}	
		}]	
	}	
}
```

# Writing Good Documentation
Good documentation should be clear and concise, but also visual, providing the following:
• A clear explanation of what the method/resource does
• Call outs that share important information with developers, including warnings and errors
• A sample call with the correlating media type body
• A list of parameters used on this resource/method, as well as their types, special formatting, rules and whether or not they are required 
• A sample response, including media type body
• Code examples for multiple languages including all necessary code (e.g. Curl with PHP, as well as examples for Java, .Net, Ruby, etc.)
• SDK examples (if SDKs are provided) showing how to access the resource/method utilizing the SDK for their language
• Interactive experiences to try/test API calls (API Console, API Notebook)
• Frequently asked questions/scenarios with code examples
• Links to additional resources (other examples, blogs, etc.)
• A comments section where users can share/discuss code
• Other support resources (forums, contact forms, etc.)
