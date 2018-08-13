# Content models for Contentful

> Example Content models made with Contentful, for Contentful users.

[Contentful](https://www.contentful.com/) is a content management platform for web applications, mobile apps and connected devices. It allows you to create, edit & manage content in the cloud and publish it anywhere via a powerful API. Contentful offers tools for managing editorial teams and enabling cooperation between organizations.

## Current Content models:
* [Blog](./blog): A simple blog example with one author, three blog entries and some images.
* [The Example App](./the-example-app): An example space simulating an online learning platform. This space is used in [The node.js example app](https://github.com/contentful/the-example-app.nodejs).

## Updating a model

To release changes, make a new git tag and a corresponding release on Github. See the two sections below for details on changing a content model and changing content. 

### Changing a model

Any breaking changes to the model should be done in a way that prevents example apps that are rendering this model from breaking. Make breaking changes by duplicating the model directory and appending the appropriate version number as a suffix to the new directory. For instance, if you want to delete a field from an entry in the `Blog` content model, please duplicate the `blog` directory with the name blog-v2 and then make the appropriate changes.

### Changing content (no model changes)

If a content change is small enough, i.e. typo fixes or minimal editing, please go ahead make your content changes in the current version(s) of the relevant export.json file. As some applications may depend on the content and different text may be considered "breaking", please version the model following the procedure described above in those situations where lots of content must be changed.
