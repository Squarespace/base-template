Template Partials
-----------------

The `/blocks/` folder contains template partials. Partials allow you to reuse code inside your template, instead of having redundant code scattered throughout your files. This can make your template easier to maintain.

### Creating a Partial

To create a partial add a `.block` file to your `/blocks/` folder. This file can contain any kind of code used in template files, most commonly HTML and JSON-T.

To use a partial in a template add a JSON-T formatter with the block file name inside the tag, like the code example below demonstrates.

    {@|apply some-block.block}

### When Should I Use Partials?

Think of partials like classes in CSS. A class is typically something that is reused across your site; classes are also broad and can be used in analogous contexts. If you will use a piece of code in your template more than once in a similar setting you may want to consider making it a partial.

### Partials and Site-Navigation

Certain Squarespace tags expect a `.block` file to provide the JSON-T for rendering that tag. (For example, the navigation tag.) To provide a partial for your site navigation, create a `.block` file here, (like `nav.block`) and then put a navigation tag in your `.region` file:

    <squarespace:navigation navigationId="siteNav" template="nav" />


### Further reading

See the squarespace docs on [Template Partials](https://developers.squarespace.com/template-partials/).
