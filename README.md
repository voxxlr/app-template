# Voxx App Template
Clone this repository to create a custom hosted App for the Voxxlr cloud platform. An App is installed via the launchpad on the Voxxlr homepage by specifying the url to an index.html. The launchpad then lets you create dedicated links to Apps using API keys that specify subsets of the data in your account. 

When serving the index.html the Voxxlr web server will fill the following mustache.js tags:

**{{key}}**
This tag contains the API key for this Sharing Link. It is required for all REST calls to app.voxxlr.com. 

**{{password}}**
If the Sharing Link has been created with password protection this tag will contain the md5 encrypted password. 

**{{og}}**
If the App has been shared with an initial document then the *og* subtags includes title, description and preview image. 

**{{{token}}}**
If the App has been shared with an initial document then this tag will contain a valid access token
