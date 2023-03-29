# Adguin
## Features
- ⚡️ Next.js 12
- ⚛️ React 18
- ⛑ TypeScript
- ✨ Styled Components - CssInJs for component styling
- 📏 ESLint — To find and fix problems in your code
- 💖 Prettier — Code Formatter for consistent style
- 🐶 Husky — For running scripts before committing
- 🚓 Commitlint — To make sure your commit messages follow the convention
- 🚫 lint-staged — Run ESLint and Prettier against staged Git files
- ⚙️ EditorConfig - Consistent coding styles across editors and IDEs
- 🗂 Path Mapping — Import components or images using the `~/` prefix
- ‽ Either Error Handler - For error handling. (Either is designed to hold either a left or a right value but never both).


## Quick Start

The best way to start with this template is using [Create Next App](https://nextjs.org/docs/api-reference/create-next-app).

```
# yarn
yarn create next-app -e https://github.com/yazaldefilimonepinto/clean-arch-nextjs-starter
# npm
npx create-next-app -e https://github.com/yazaldefilimonepinto/clean-arch-nextjs-starter
```

### Development

To start the project locally, run:

```bash
  npm dev
  our
  yarn dev
```

Open `http://localhost:3000` with your browser to see the result.


### Requirements

- Node.js >= 12.22.0
- npm our yarn

### Directory Structure

- [`.husky`](.husky) — Husky configuration and hooks.<br>
- [`public`](./public) — Static assets such as robots.txt, images, and favicon.<br>
- [`src`](./src) — Application source code, including pages, components, styles.<br>

### Scripts
- `yarn/npm dev` — Starts the application in development mode at `http://localhost:3000`.
- `yarn/npm build` — Creates an optimized production build of your application.
- `yarn/npm start` — Starts the application in production mode.
- `yarn/npm lint` — Runs ESLint for all files in the `src` directory.


Folder Structure Conventions
============================

> Folder structure options and naming conventions for software projects

### A typical top-level directory layout

    .
    ├── build                   # Compiled files (alternatively `dist`)
    ├── docs                    # Documentation files (alternatively `doc`)
    ├── src                     # Source files (alternatively `lib` or `app`)
    ├── test                    # Automated tests (alternatively `spec` or `tests`)
    ├── tools                   # Tools and utilities
    ├── LICENSE
    └── README.md

> Use short lowercase names at least for the top-level files and folders except
> `LICENSE`, `README.md`

### Source files

The actual source files of a software project are usually stored inside the
`src` folder. Alternatively, you can put them into the `lib` (if you're
developing a library), or into the `app` folder (if your application's source
files are not supposed to be compiled).

> **Samples**: [jQuery](https://github.com/jquery/jquery) `src`, [Node.js](https://github.com/nodejs/node) `lib` and `src`, [D3.js](https://github.com/mbostock/d3) `src`, [AngularJS](https://github.com/angular/angular.js) `src`, [Adobe Brackets](https://github.com/adobe/brackets) `src`, [three.js](https://github.com/mrdoob/three.js) `src`, [Express](https://github.com/visionmedia/express) `lib`, [Socket.IO](https://github.com/LearnBoost/socket.io) `lib`, [Less.js](https://github.com/less/less.js) `lib`, [Redis](https://github.com/antirez/redis) `src`, [Ace](https://github.com/ajaxorg/ace) `lib`, [Semantic UI](https://github.com/Semantic-Org/Semantic-UI) `src`, [Zepto.js](https://github.com/madrobby/zepto) `src`, [Emscripten](https://github.com/kripken/emscripten) `src`, [RethinkDB](https://github.com/rethinkdb/rethinkdb) `src`, [Bitcoin](https://github.com/bitcoin/bitcoin) `src`, [MongoDB](https://github.com/mongodb/mongo) `src`, [Facebook React](https://github.com/facebook/react) `src`, [Rust](https://github.com/mozilla/rust) `src`, [ASP.NET](https://aspnetwebstack.codeplex.com/SourceControl/latest) `src`, [SignalR](https://github.com/SignalR/SignalR) `src`, [libgit2](https://github.com/libgit2/libgit2) `src`

### Automated tests

Automated tests are usually placed into the `test` or, less commonly, into the `spec` or `tests` folder.

> **Q: Why tests are placed into a separate folder, as opposed to having them closer to the code under test?**
>
> **A:** Because you don't want to test the code, you want to test the *program*.

    .
    ├── ...
    ├── test                    # Test files (alternatively `spec` or `tests`)
    │   ├── benchmarks          # Load and stress tests
    │   ├── integration         # End-to-end, integration tests (alternatively `e2e`)
    │   └── unit                # Unit tests
    └── ...

> **Samples**: [jQuery](https://github.com/jquery/jquery), [Node.js](https://github.com/joyent/node), [D3.js](https://github.com/mbostock/d3), [AngularJS](https://github.com/angular/angular.js), [Adobe Brackets](https://github.com/adobe/brackets), [three.js](https://github.com/mrdoob/three.js), [Express](https://github.com/visionmedia/express), [Socket.IO](https://github.com/LearnBoost/socket.io), [Less.js](https://github.com/less/less.js), [Bower](https://github.com/bower/bower), [Mozilla PDF.js](https://github.com/mozilla/pdf.js), [Grunt](https://github.com/gruntjs/grunt), [Gulp](https://github.com/gulpjs/gulp), [Semantic UI](https://github.com/Semantic-Org/Semantic-UI), [Zepto.js](https://github.com/madrobby/zepto), [Jade](https://github.com/visionmedia/jade), [RethinkDB](https://github.com/rethinkdb/rethinkdb), [Vagrant](https://github.com/mitchellh/vagrant), [Sails.js](https://github.com/balderdashy/sails), [GitHub Hubot](https://github.com/github/hubot), [Facebook React](https://github.com/facebook/react), [Ansible](https://github.com/ansible/ansible), [ASP.NET](https://aspnetwebstack.codeplex.com/SourceControl/latest), [browserify](https://github.com/substack/node-browserify), [Paper.js](https://github.com/paperjs/paper.js), [Julia](https://github.com/JuliaLang/julia), [Karma](https://github.com/karma-runner/karma)

### Documentation files

Often it is beneficial to include some reference data into the project, such as
Rich Text Format (RTF) documentation, which is usually stored into the `docs`
or, less commonly, into the `doc` folder.

    .
    ├── ...
    ├── docs                    # Documentation files (alternatively `doc`)
    │   ├── TOC.md              # Table of contents
    │   ├── faq.md              # Frequently asked questions
    │   ├── misc.md             # Miscellaneous information
    │   ├── usage.md            # Getting started guide
    │   └── ...                 # etc.
    └── ...

> **Samples**: [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate) `doc`, [Backbone](https://github.com/jashkenas/backbone) `docs`, [three.js](https://github.com/mrdoob/three.js) `docs`, [GitLab](https://github.com/gitlabhq/gitlabhq) `doc`, [Underscore.js](https://github.com/jashkenas/underscore) `docs`, [Discourse](https://github.com/emberjs/ember.js) `docs`, [Grunt](https://github.com/gruntjs/grunt) `docs`, [Emscripten](https://github.com/kripken/emscripten) `docs`, [RethinkDB](https://github.com/rethinkdb/rethinkdb) `docs`, [RequireJS](https://github.com/jrburke/requirejs) `docs`, [GitHub Hubot](https://github.com/github/hubot) `docs`, [Twitter Flight](https://github.com/flightjs/flight) `doc`, [Video.js](https://github.com/videojs/video.js) `docs`, [Bitcoin](https://github.com/bitcoin/bitcoin) `doc`, [MongoDB](https://github.com/mongodb/mongo) `docs`, [Facebook React](https://github.com/facebook/react) `docs`, [libgit2](https://github.com/libgit2/libgit2) `docs`, [Stylus](https://github.com/LearnBoost/stylus) `docs`, [Gulp](https://github.com/gulpjs/gulp) `docs`, [Brunch](https://github.com/brunch/brunch) `docs`

### Scripts

...

### Tools and utilities

...

### Compiled files

...

### 3rd party libraries

...
