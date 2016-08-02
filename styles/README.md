Styles
------

This folder contains the LESS and CSS styles for your website. All Squarespace styles are processed using [LESS](http://lesscss.org/). LESS extends CSS with dynamic behavior such as variables, mixins, operations and functions.

To include CSS or LESS files in your template, edit the template.conf and list the files in the order you wish to include them. For example:

    "stylesheets" : [ "global.css", "my-site.less", "another-style.less" ]

All stylesheets added to the template.conf in this way will be compiled and served as one CSS file automatically. You do not need to add any stylesheet links to the HEAD section of your site.

> NOTE: If you add a file named reset.css to the /styles folder it will automatically be added to the top of the site.css file and it should not be listed in the stylesheets variable in the template.conf file.

### Further Reading

For further reading, see the [Template Overview documentation](https://developers.squarespace.com/template-overview/). To read about adding attributes to our style editor, see the [Style Editor documentation](https://developers.squarespace.com/style-editor/).
