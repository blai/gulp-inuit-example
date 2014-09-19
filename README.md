# gulp-inuit-example

This sample project is generated using [generator-gulp-webapp](https://github.com/yeoman/generator-gulp-webapp), with the only modification being the `styles` task inside `gulpfile.js`, and some additional `.scss` files to show how `gulp-inuit` work.

It packages all the Inuit components listed under [here](https://github.com/inuitcss), through bower dependency specified in `bower.json`.

Any local style implementation should take place under `app/styles/`. You can add/remove any `.scss` file there and expect the `gulp-inuit` plugin to handle the sorting according to the [Inuit Getting started guide](https://github.com/inuitcss/getting-started#import-order). If your `.scss` file name begines with `_customize.` (or `customize.`), it would be imported before all default Inuit sections, this allows you to override the variables provided by various Inuit modules. If your `.scss` file name does not contain any recognizable Inuit section name (or `_customzie.`), it will be imported at last.

## See it in action

```
git clone git@github.com:blai/gulp-inuit-example.git
cd gulp-inuit-example
npm install
bower install
gulp serve
```

Running the above would launch a web page with some default contents, plus some demo stylings in `app/styles/`. You should also be able to find the aggregated `.scss` main file under `.tmp/styles/main.scss`, the compiled file is `main.css`.

You can also add/remove any Inuit modules using bower, and rerun the command to see the changes.
