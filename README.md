Atlas Plugins
=================

This is a repository that holds JS plugins to be used in Atlas. Each plugin will have its own folder, with test coverage. It is also expected that each plugin has a `README.md` file, to explain how the plugin is to be used.


Writing a plugin
--------------------

1. Create a new folder named after the plugin inside of `/plugins`
2. Create a `package.json` file to specify the version number. We borrowed this from NPM, but we're only using the file to track the dependencies and version number.
3. Write a bunch of coffeescript files. Yay!
4. Create a `README.md` file that describes how to use the plugin.


Testing a plugin
----------------


Building a plugin
-----------------

Run the `gulp build` command to build all plugins into the `/build` folder. Then upload the resulting file to the `orm-atlas-plugins` bucket on S3, and access the file on the Cloudfront CDN on `d2uogd9jz9k9zm.cloudfront.net`.