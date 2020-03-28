## To-do App Overview

These tutorials demonstrate how to use Stitch to integrate
[Atlas](https://docs.mongodb.com/stitch/mongodb/), [Authentication providers](https://docs.mongodb.com/stitch/authentication/providers/),
and [external services](https://docs.mongodb.com/stitch/services/) to build a To-Do app.

You will start by building the Stitch backend. From there, you can download
the code for one or more of the platforms and see how users can create and maintain
individual to-do lists on multiple platforms.

## To-do App Architecture[¶](https://docs.mongodb.com/stitch/tutorials/todo-overview/#to-do-app-architecture "Permalink to this headline")

The following image shows the final application architecture:

![../../_images/todo_overview.png](https://docs.mongodb.com/stitch/_images/todo_overview.png)

In the first tutorial, you will set up the backend to use Anonymous
authentication and you will configure Rules for the two collections. You can then
build one or more client apps that connect to the backend. In later tutorials,
you will add the additional features to both the backend and client apps.

The `To-Do` app uses the `items` collection in the `todo`
database, and stores one document per each to-do item. A to-do item has the following
format:

<pre>
{
   _id : ObjectId("5be2118cc6eda6d1671ddee3"),
   owner_id : ObjectId("5be1158f4ffdc28344840ae4"),
   text : "Put your right foot in.",
   checked : true,
   __stitch_sync_version : {
      spv : 1,
      id : "c73dd901-bba3-44ab-bf49-9b8abc99c7d1",
      v : 3
   }
}
</pre>
