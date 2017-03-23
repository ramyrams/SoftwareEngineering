# Identifier Design with URIs

URI Format

* Rule: Forward slash separator (/) must be used to indicate a hierarchical relationshi
```xml
http://api.canvas.restapi.org/shapes/polygons/quadrilaterals/squares
```
* Rule: A trailing forward slash (/) should not be included in URIs
```xml
Many web components and frameworks will treat the following two URIs equally:
http://api.canvas.restapi.org/shapes/
http://api.canvas.restapi.org/shapes
```

* Rule: Hyphens (-) should be used to improve the readability of URIs
```xml
http://api.example.restapi.org/blogs/mark-masse/entries/this-is-my-first-post
```

* Rule: Underscores (_) should not be used in URIs 
* Rule: Lowercase letters should be preferred in URI paths 
* Rule: File extensions should not be included in URIs 
```xml
http://api.college.restapi.org/students/3248234/transcripts/2005/fall.json (not prefered)
http://api.college.restapi.org/students/3248234/transcripts/2005/fall 
```

# URI Authority Design
* Rule: Consistent subdomain names should be used for your APIs
```
For example:
http://api.soccer.restapi.org
```
* Rule: Consistent subdomain names should be used for your client developer portal


# Resource Modeling
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
* Rule: A singular noun should be used for document names 
For example, the URI for a single player document would have the singular form:
http://api.soccer.restapi.org/leagues/seattle/teams/trebuchet/players/claudio

* Rule: A plural noun should be used for collection names 
For example, the URI for a collection of player documents uses the plural noun form of its contained resources:
http://api.soccer.restapi.org/leagues/seattle/teams/trebuchet/players

* Rule: A plural noun should be used for store names 
The URI for a store of music playlists may use the plural noun form as follows:
http://api.music.restapi.org/artists/mikemassedotcom/playlists

* Rule: A verb or verb phrase should be used for controller names 
 For example:
http://api.college.restapi.org/students/morgan/register
http://api.example.restapi.org/lists/4324/dedupe
http://api.ognom.restapi.org/dbs/reindex
http://api.build.restapi.org/qa/nightly/runTestSuite


* Rule: Variable path segments may be substituted with identity-based values 
 The URI template example below has three variables (leagueId, TeamId, and playerId):
http://api.soccer.restapi.org/leagues/{leagueId}/teams/{teamId}/players/{playerId}

http://api.soccer.restapi.org/leagues/seattle/teams/trebuchet/players/21 - Conceptually, the value 21 occupies a variable path segment slot named playerId.
http://api.soccer.restapi.org/games/3fd65a60-cb8b-11e0-9572-0800200c9a66 - The UUID value fills in the gameId variable.

* Rule: CRUD function names should not be used in URIs 
For example, this API interaction design is preferred:
DELETE /users/1234

The following anti-patterns exemplify what not to do:
GET /deleteUser?id=1234
GET /deleteUser/1234
DELETE /deleteUser/1234
POST /users/1234/delete

# URI Query Design 
* Rule: The query component of a URI may be used to filter collections or stores 
* Rule: The query component of a URI should be used to paginate collection or store results 
