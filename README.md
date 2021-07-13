# Voxxlr App Template
Clone this repository to create a custom hosted App for the Voxxlr cloud platform. Install the App via the launchpad on the Voxxlr homepage by entering the url to the index.html. The launchpad then lets you create dedicated _links_ to the Apps using API keys that specify subsets of the data in your account. When serving the index.html the Voxxlr web server provides the following mustache.js tags. The index.html in this repository provides an example of how the tags are used to configure and App.

---
**{{key}}**

This tag contains the API key for a given _link_. It is required for REST calls to [https://app.voxxlr.com](https://app.voxxlr.com/rest.html). 

---
**{{password}}**

If a _link_ is password protected then this tag will contain the md5 encrypted password. 

---
**{{og}}**

If a _link_ loads an initial document then the *og* subtags includes title, description and preview image. 

---
**{{{token}}}**

If a _link_ loads an initial document then this tag will contain a valid access token.

---
**{{{launchpad}}}**

The launchpad tag is only present if an App is opened via the launchpad on the homepage. 
