# DS-GA 1003 Website

## Development info

### Technologies used

[Stylus](https://learnboost.github.io/stylus/) is used for styling.

[Travis](https://travis-ci.org/) is used to build and deploy the website to gh-pages on each push, per [this guide](https://gist.github.com/domenic/ec8b0fc8ab45f39403dd).

The site is intended to be responsive, which we accomplish with per-device stylesheets and media queries in the HTML.

Ideally while editing you should be using an [EditorConfig](http://editorconfig.org/) plugin for your text editor to enforce a few basic stylistic things.

We are trying to maintain a reasonable HTML document outline (so, don't use `<section>` as if it were `<div>`). To preview the document outline, use the [HTML 5 Outliner tool](https://gsnedders.html5.org/outliner/); here's [a direct link to the outline for the current version](https://gsnedders.html5.org/outliner/process.py?url=https%3A%2F%2Fdavidrosenberg.github.io%2Fml2015%2F%23home).

### Building locally

Be sure to have [io.js](https://iojs.org/) installed. (Node.js will do if you feel like rockin' in 2013 style.)

Run `npm install` in the project root. This will install some build tools we use.

Run `npm run watch` to start a watcher that will compile things in place. You can then view the site by simply opening `index.html`.

Run `npm run build` to do a local build into the `out/` directory. You can then preview the site at `out/index.html`. This should usually be the same as just `index.html`, but it is good to check before committing, since the build process is slightly more complicated than the in-place watch process.