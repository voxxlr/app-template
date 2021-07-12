# Voxx App Template
Clone this repository to create a custom hosted App for the Voxxlr cloud platform. An App is installed via the launchpad on the Voxxlr homepage by specifying the url to an index.html. The launchpad then lets you create dedicated _links_ to Apps using API keys that specify subsets of the data in your account. When serving the index.html the Voxxlr web server will fill the following mustache.js tags:

---
**{{key}}**

This tag contains the API key for a given _link_. It is required for all REST calls to app.voxxlr.com. 

---
**{{password}}**

If a _link_ has been created with a password protection then this tag will contain the md5 encrypted password. 

---
**{{og}}**

If the App has been shared with an initial document then the *og* subtags includes title, description and preview image. 

---
**{{{token}}}**

If the App has been shared with an initial document then this tag will contain a valid access token.

---
**{{{launchpad}}}**

The launchpad tag is only present if an App is opened via the launchpad on the homepage. 
