# gulp-inuit-example

This sample project is generated using [generator-gulp-webapp](https://github.com/yeoman/generator-gulp-webapp). It has the following modifications:

* `style` task inside `gulpfile.js` is change to use `gulp-inuit`.
* added `customize-inuit` task, which, when you run `gulp customize-inuit`, will generate a set of `_customize.section.module.scss` files under `app/styles/customize`. `_customize.settings.default.scss` is customized to show case the customization actually works, all Inuit module features are turned on.
* `app/index.html` is filled with a kitchen sink like tests for all the styles Inuit affects.
* Added all Inuit components listed under [here](https://github.com/inuitcss), through bower dependency specified in `bower.json`.

## See it in action

### Run kitchen sink test

```
git clone git@github.com:blai/gulp-inuit-example.git
cd gulp-inuit-example
npm install
bower install
gulp watch
```

### Try the `customize-inuit` task

```
gulp customize-inuit
```

Since I have run this command once checked in the generated files, when you run this command, a command prompt would be displayed for those files that I have changed, this shows you how you can safely run the command over and over again, even after you have modified the `_customize...scss` files (think: when you update an Inuit module, and the update introduced new variables).
