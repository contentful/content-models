Content model: `The Example App`
================================

The example app content model containts the model for all the example apps, demonstrating in a broader fashion some examples on how to use
Contentful. If you want to see the model in action, we have a [hosted version](https://the-example-app-nodejs.herokuapp.com/), for you
to check out.

Through our [command line app](https://github.com/contentful/contentful-cli) you can import this model into your own space. Doing so will be
accomplished by this call to the command line app:

```
contentful space seed -s '<SPACE_ID>' -t the-example-app
```

The Contentful CLI will walk you through the steps needed in order to import this content model into your space.

If you happen to not have a `<SPACE_ID>`, as in a Space you can overwrite, use the cli to create a new one:

```
contentful space create -n '[COPY] The example app'
```

And then retry the upper code again.



Other apps
==========

The Node example app is not the only one. Soon™ there will be more available, all using the
same space.

Stay tuned for updates on the model and example apps.



Versions
========

We are hosting versions of this content model for demo purposes. `The Example App` can be connected to these versions through `variables.env` when run locally or through query paramters when hosted. For example: https://the-example-app-nodejs.herokuapp.com/?space_id=<YOUR_CLONED_SPACE_ID>&delivery_token=<YOUR_DELIVERY_TOKEN>&preview_token=<YOUR_PREVIEW_TOKEN>

| Version  | Space Id | Content Delivery API - access token | Content Preview API - access token |
| - | - | - | - |
| 1.0 | `ft4tkuv7nwl0` | `57459fe48bd2b1bef4855294455af52562dbc0c7f0eb84f8b2cd68692c186417` | `a9972e3cd83528def2fc9d3428c67cd622eb26d0a24239718c6ac61fe0288f2f` |

**Note:** We are sharing read-only tokens here for demo purposes. Tokens should in general be treated like passwords and not shared with a public audience.

Visual graph of content model
=============================
Using [contentful-graph](https://www.npmjs.com/package/contentful-graph) the following graph was generated to visualize the content model.
![graph of content model](https://raw.githubusercontent.com/contentful/content-models/master/the-example-app/the-example-app-space-v1.png)
