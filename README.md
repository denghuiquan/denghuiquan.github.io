# pages-boilerplate

[![Build Status][travis-image]][travis-url]
[![Package Version][version-image]][version-url]
[![License][license-image]][license-url]
[![Code Style][style-image]][style-url]

> Always a pleasure scaffolding your awesome static sites.

## Getting Started

```shell
# clone repo
$ git clone https://github.com/denghuiquan/denghuiquan.github.io.git my-awesome-pages
$ cd my-awesome-pages
# install dependencies
$ yarn # or npm install
```

## Usage

```shell
$ yarn <task> [options]
```

### e.g.

```shell
# Runs the app in development mode
$ yarn serve --port 5210 --open
# Builds the app for production to the `dist` folder
$ yarn build --production
```

### Available Scripts

#### `yarn lint` or `npm run lint`

Lint the styles & scripts files.

#### `yarn compile` or `npm run compile`

Compile the styles & scripts & pages file.

#### `yarn serve` or `npm run serve`

Runs the app in development mode with a automated server.

##### options

- `open`: Open browser on start, Default: `false`
- `port`: Specify server port, Default: `2080`

#### `yarn build` or `npm run build`

Builds the app for production to the `dist` folder. It minify source in production mode for the best performance.

##### options

- `production`: Production mode flag, Default: `false`
- `prod`: Alias to `production`

#### `yarn start` or `npm run start`

Running projects in production mode.

##### options

- `open`: Open browser on start, Default: `false`
- `port`: Specify server port, Default: `2080`

#### `yarn deploy` or `npm run deploy`

Deploy the `dist` folder to [GitHub Pages](https://pages.github.com).

##### options

- `branch`: The name of the branch you'll be pushing to, Default: `'gh-pages'`

#### `yarn clean` or `npm run clean`

Clean the `dist` & `temp` files.

> **NOTE**: If you need to run script with options, you can add them for yarn command like this `yarn start --port 8080 --open true`; and you can add for npm command like `npm run start -- --port 8080 --open true` 

## Folder Structure

```
└── my-awesome-pages ·································· project root
   ├── public ········································· static folder
   │   └── favicon.ico ································ static file (unprocessed)
   ├── src ············································ source folder
   │   ├── assets ····································· assets folder
   │   │   ├── fonts ·································· fonts folder
   │   │   │   ├── pages.eot ·························· font file (imagemin)
   │   │   │   ├── pages.svg
   │   │   │   ├── pages.ttf
   │   │   │   └── pages.woff
   │   │   ├── images ································· images folder
   │   │   │   ├── brands.svg ························· image file (imagemin)
   │   │   │   └── logo.png
   │   │   ├── scripts ································ scripts folder
   │   │   │   └── main.js ···························· script file (babel / uglify)
   │   │   └── styles ································· styles folder
   │   │       ├── _icons.scss
   │   │       ├── _variables.scss ···················· partial sass file (dont output)
   │   │       └── main.scss ·························· entry scss file (scss / postcss)
   │   ├── layouts ···································· layouts folder
   │   │   └── basic.html ····························· layout file (dont output)
   │   ├── partials ··································· partials folder
   │   │   ├── footer.html
   │   │   └── header.html ···························· partial file (dont output)
   │   ├── about.html ································· page file (use layout & partials)
   │   └── index.html ································· page file (use layout & partials)
   ├── .editorconfig ·································· editor config file
   ├── .gitignore ····································· git ignore file
   ├── .npmrc
   ├── .travis.yml ···································· travis ci config file
   ├── LICENSE ········································ repo license
   ├── README.md ······································ repo readme
   ├── gulpfile.js ···································· gulp tasks file
   ├── package-lock.json
   ├── package.json ··································· package file
   └── yarn.lock ······································ yarn lock file
```

## Related

## Contributing

1. **Fork** it on GitHub!
2. **Clone** the fork to your own machine.
3. **Checkout** your feature branch: `git checkout -b my-awesome-feature`
4. **Commit** your changes to your own branch: `git commit -am 'Add some feature'`
5. **Push** your work back up to your fork: `git push -u origin my-awesome-feature`
6. Submit a **Pull Request** so that we can review your changes.

> **NOTE**: Be sure to merge the latest from "upstream" before making a pull request!

## License

[MIT](LICENSE) &copy; [denghuiquan](https://github.com/denghuiquan)


[version-image]: https://img.shields.io/github/package-json/v/denghuiquan/denghuiquan.github.io/master.svg
[version-url]: https://github.com/denghuiquan/denghuiquan.github.io
[license-image]: https://img.shields.io/github/license/denghuiquan/denghuiquan.github.io.svg
[license-url]: https://github.com/denghuiquan/denghuiquan.github.io/blob/master/LICENSE
[style-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[style-url]: http://standardjs.com
