Collections
-----------

This folder contains collection definitions. Collections allow you to group together a set of pages, like a gallery, blog or album. Collections are JSON-T templates that determine how data on your site is rendered. Each collection should have a configuration file (`.conf`) and a `.item` and/or `.list` file.

### Collection Configuration (collection.conf)

Contains the configuration settings for a collection. There is one configuration file for each collection.

    {
      "title" : "Blog",
      "ordering" : "chronological",
      "addText" : "Add Post",
      "acceptTypes" : [ "text" ]
    }

#### Configuration Options

- **title**: The name of the collection as it will appear in the "Add New Page" dialog.
- **ordering**: The method of ordering for the collection. Available options: chronological, user-orderable, calendar.
- **addText**: Specifies the text used in the "add" button in the Squarespace interface. It is also used in empty collection message when a collection does not contain any items.
- **acceptTypes**: Specifies the post types allowed in this collection. Available: text, image, video.

### Collection List Views (collection.list)

This is the default view of every collection and shows all posts in that collection. For example, `blog.list` templates a list of blog posts.

Each `.list` template will have access to the top level `items` key in its context. This is a list of all the items in the collection. To explore the context for a collection list view, visit any existing blog or gallery page using the `?format=json-pretty` query parameter. (For example, [http://base-template.squarespace.com/blog?format=json-pretty](http://base-template.squarespace.com/blog?format=json-pretty))

### Collection Item Views (collection.item)

Item views are templates for the individual pages of a collection. Example: blog.item templates a single blog post page. 

Each `.item` template will have access to the `item` key in its context. This will contain data attributes relevant to that item. To explore the context for a collection item view, visit any existing blog post or gallery image page using the `?format=json-pretty` query parameter. 

### Further Reading

For further help, consult the [Collections page](https://developers.squarespace.com/collections/) in the developer docs.
