# gulp-boilerplate
My own Gulp boilerplate for developing static webpages and deploying on GitHub Pages.
It has two main tasks **serve (deafult) task** for development and **deploy task** for GitHub Pages deployment.
It was originally created to be used during wegielpruszkow-v2 development.

#### Serve task:
* watches .html, .scss and .js files,
* lints .js files and logs errors to terminal,
* checks Sass files and logs errors to terminal,
* reloads on markup, styles' and scripts' change (life reload with BrowserSync).

#### Deploy task:
* removes old dist directory (if existing),
* creates new dist directory for deployment,
* compiles Sass files,
* copies fonts to dist directory,
* bundles multiple .css files,
* minifies .css file,
* bundles multiple .js files,
* uglifies .js file,
* creates new index.html file with one bundled .css and .js file respectively,
* minifies and caches images,
* asks for commit message,
* pushes changes to remote `gh-pages` branch with given commit message.

#### Technologies
* Sass,
* Skeleton CSS framework/ boilerplate,
* Gulp

#### Installation
Reqires [Node.js](https://nodejs.org/en/).
Instal devDependencies and start the server.
```
$ cd gulp-boilerplate
$ npm install
$ gulp serve
```

For deployment run
```
$ gulp deploy
```

#### License
unlicensed

_**TODO:** Add ES6 support._ 
