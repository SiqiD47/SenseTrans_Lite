## Code Structure

The main portion of this Chrome extension is written in bundle.js.

There are 7 modules in this file, indexed with 1~7. The npm modules include: compromise (module 2), node-ner (module 3), underscore (module 4), vader-sentiment (module 5), path (module 6), _process (module 7). The main functions of this Chrome extension can be found in module 1.

Generally, using these modules in Javascript only requires an 'npm install xxx' command in the terminal followed by another command 'require('xxx')' in the js file. However, this cannot be accomplished in the browser. Thus, we used Browserify (http://browserify.org/) to enable us to require('modules') in the browser by bundling up all of the dependencies.


# To bundle up the project:

First install node, which ships with npm. Then do: npm install -g browserify