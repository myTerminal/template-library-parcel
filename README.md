# template-library-parcel

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0)

A template to create front-end libraries with [Parcel.js](https://parceljs.org) as the bundler [in-progress]

## Technologies

### Web

 - [jQuery](https://jquery.com/) (sample dependency)
 - [ES2015](http://es6-features.org/)
 - [Less CSS](http://lesscss.org/)

### Module bundler: Parcel

All you need is [parcel-bundler](https://www.npmjs.com/package/parcel-bundler) and it takes care of almost everything implicitly.

#### A few other packages

 - [babel-preset-env](https://www.npmjs.com/package/babel-preset-env) to transpile ES2015 scripts to regular JavaScript but no [babel-core](https://www.npmjs.com/package/babel-core)!
 - [less](https://www.npmjs.com/package/less) to help parcel-bundler with transpilation of Less CSS into regular CSS (if you do not include this, parcel-bundle automatically adds it)
 - [effortless-css](https://www.npmjs.com/package/effortless-css) to provide Less CSS mixins
 - [eslint](https://www.npmjs.com/package/eslint) for running ESLint to lint JavaScript files
 - [babel-eslint](https://www.npmjs.com/package/babel-eslint), [eslint-config-myterminal](https://www.npmjs.com/package/eslint-config-myterminal), [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb), [eslint-plugin-import](https://www.npmjs.com/package/eslint-plugin-import), [eslint-plugin-jsx-a11y](https://www.npmjs.com/package/eslint-plugin-jsx-a11y) and [eslint-plugin-react](https://www.npmjs.com/package/eslint-plugin-react) to support eslint

#### Commands

 - `npm run develop` to instruct parcel-bundler to build the library and keep watching for file changes within the source.
 - `npm run build` to instruct parcel-bundler to build the library and stop.  
 - `npm run lint` to run ESLint on all JavaScript source files.

## To-Do

 - Find a way to separate other content like fonts, etc.
 - Find a way to exclude external dependencies
 - Find a way to generate source-maps
 - Find a way to build UMD modules
 - Find a way to write and run tests
