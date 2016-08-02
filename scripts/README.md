Custom Javascript
-----------------

You can use any custom javascript file or library in your Squarespace Template. Squarespace provides a script loader that minifies and combines your custom scripts, which you can use if you like. Alternatively you can package your scripts using the preprocessor of your choice.

### Using the Script Loader

Squarespace's script loader minifies your code and allows you to combine all of your JavaScript files into one, cutting down on HTTP requests. Loading JavaScript in Squarespace is very similar to the standard script tag syntax in HTML. The syntax is outlined in the code sample below.

    <squarespace:script src="plugin.js" combo="true" />
    <squarespace:script src="site.js" combo="true" />

> NOTE: The script's src path is relative to the template /scripts folder.

### Using your own Javascript Preprocessor

You can use any javascript workflow tool, like NPM, gulp, browserify or webpack. You can include the compiled code in your /scripts folder, and link to those files using regular script tags, or the Squarespace Script Tag.

### Further Reading

For further reading, check out the [Squarespace developer docs on Javascript](https://developers.squarespace.com/custom-javascript/).