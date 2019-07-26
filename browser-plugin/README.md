## Mule Preview Browser Extension

### Summary

This project takes the [Mule Preview client](../client)
and uses it to replace a diff of Mule XML in Bitbucket
with a graphical diff.

### Instructions

Simply open a PR in Bitbucket and select a Mule XML file.
The Mule Preview button in your browsers toolbar should enable.
Clicking it will toggle Mule Preview mode.

### Support

Only tested on Firefox but it should also be compatible with Chrome.

### Building

Simply run these command to produce a production build

    $ npm install
    $ npm run prebuild
    $ npm run build

Note: This is currently broken because UglifyJs doesn't like the output of Babel at the moment.

### Developing

This commands set you up for development:

    $ npm install
    $ npm prebuild

This command will build the plugin and rebuild if any files change:

    $ npm start

This command will hot reload the extension into Firefox

    $ npx web-ext run -s extension/

This command will ensure your code is up to scratch before comitting.

    $ npm run lint

### Acknowledgement

Thanks to https://github.com/williankeller/browser-extension-boilerplate for making this extension so easy to get running.