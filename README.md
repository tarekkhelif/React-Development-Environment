# Development Environment for React with JSX

This is my setup for web development with React using VSCode.

## Overview

There are [linting/formatting tools](#lint) to help write correct & pretty code, [language extensions](#extensions) to do cool things, [development tools](#dev) to automatically see updates and to make debugging easier, and a [build pipeline](#build) to transpile code down to ES5 and bundle it into a small number of files. There's also a [git repository](#vcs) included.

### <a id="lint"></a>Linting and formatting

* **ESLint** and **Prettier** and set up to work with their corresponding VSCode extensions to _indicate errors_ as you type and to _auto-format_ code on save.
* **Stylelint** and **Prettier** do the _same for CSS/SCSS_.
* **Flow** checks for _type errors_.

### <a id="extensions"></a>Language Extensions

* **Webpack** allows all sorts of files (CSS, images, etc.) to be _imported into JS modules_.
* Babel extends JavaScript with **JSX** to make React components easier to deal with.
* **Flow**'s _type annotations_ are non-standard JavaScript and are stripped out during transpilation using Babel.
* **Sass** (in the form of _SCSS_), essentially an extension of CSS, can be used for styling instead of CSS.

### <a id="dev"></a>Development Tools

* **Webpack**'s dev server _automatically reloads pages_ when code changes and _hot module replacement_ is installed to update certain pieces of a page without refreshing the whole thing.
* VSCode's **Chrome debugger** allows an app running in Chrome to be _debugged within VSCode_.
* **Webpack** generates _source maps_ for the code it transpiles and bundles so the debugger can _reference line numbers in the source code_ rather than the transpiled and bundled code that's actually running.

### <a id="build"></a>Build Pipeline

* **Webpack** and **Babel** _transpile source code down to ES5_, removing language extensions and converting post-ES5 syntax to ES5.
* **Babel**'s polyfill enables post-ES5 APIs
* **Webpack** _bundles code_ that's organized into separate modules into a single file.
* **Webpack** takes all the files required for the app (code, style, images, etc.) and puts them into a _`dist/` folder for distribution_.

### <a id="vcs"></a>Version Control

* **Git** is used for _version control_. The assembly of this set up is included in the git history.
