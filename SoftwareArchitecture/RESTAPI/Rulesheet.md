# Identifier Design with URIs

URI Format

Rule: Forward slash separator (/) must be used to indicate a hierarchical relationshi
http://api.canvas.restapi.org/shapes/polygons/quadrilaterals/squares

Rule: A trailing forward slash (/) should not be included in URIs

Many web components and frameworks will treat the following two URIs equally:
http://api.canvas.restapi.org/shapes/
http://api.canvas.restapi.org/shapes


Rule: Hyphens (-) should be used to improve the readability of URIs
http://api.example.restapi.org/blogs/mark-masse/entries/this-is-my-first-post

Rule: Underscores (_) should not be used in URIs 
Rule: Lowercase letters should be preferred in URI paths 
Rule: File extensions should not be included in URIs 
http://api.college.restapi.org/students/3248234/transcripts/2005/fall.json (not prefered)
http://api.college.restapi.org/students/3248234/transcripts/2005/fall 

URI Authority Design
Rule: Consistent subdomain names should be used for your APIs
For example:
http://api.soccer.restapi.org
Rule: Consistent subdomain names should be used for your client developer portal


Resource Modeling


The URI path conveys a REST API’s resource model, with each forward slash separated
path segment corresponding to a unique resource within the model’s hierarchy. For
example, this URI design:
http://api.soccer.restapi.org/leagues/seattle/teams/trebuchet
indicates that each of these URIs should also identify an addressable resource:
http://api.soccer.restapi.org/leagues/seattle/teams
http://api.soccer.restapi.org/leagues/seattle
http://api.soccer.restapi.org/leagues
http://api.soccer.restapi.org


# URI Path Design

# URI Path Design 
Rule: A singular noun should be used for document names 
Rule: A plural noun should be used for collection names 
Rule: A plural noun should be used for store names 
Rule: A verb or verb phrase should be used for controller names 
Rule: Variable path segments may be substituted with identity-based values 
Rule: CRUD function names should not be used in URIs 

# URI Query Design 
Rule: The query component of a URI may be used to filter collections or stores 
Rule: The query component of a URI should be used to paginate collection or store results 
