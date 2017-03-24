
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
