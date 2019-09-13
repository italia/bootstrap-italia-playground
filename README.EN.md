# Bootstrap Italia Playground

This little project is the easiest way to start playing with [Bootstrap Italia](https://italia.github.io/bootstrap-italia/).

<img src="https://github.com/italia/bootstrap-italia-playground/blob/master/bootstrap-italia-playground.png" width="800"> 

## What's included

You'll find a plain HTML page linking Bootstrap Italia files and empty CSS and JS files to enable styling.

```
bootstrap-italia-playground/
│   index.html          # main html file
├── css/
│   ├── main.css        # working CSS file
└── js/
    └── main.js         # working JS file
```

## Getting started

* Clone the repo: `git clone https://github.com/italia/bootstrap-italia-playground.git`
* Install dependencies: `yarn install`
* Run a local server: `yarn start`
* Point a browser to: `http://127.0.0.1:8080/`

## Updating Bootstrap Italia colours

To update Bootstrap Italia primary colour, please refer to the `scss/main.scss` file, where `$primary` colour variable is overridden.  
To build a customised version of the library:

* Build a custom Bootstrap Italia CSS file with `yarn buildCSS`
* Comment out original Bootstrap Italia CSS `<link href="/node_modules/bootstrap-italia/dist/css/bootstrap-italia.min.css" rel="stylesheet">`
* Uncomment Bootstrap Italia custom CSS `<link href="/css/bootstrap-italia-custom.min.css" rel="stylesheet">`

Just run `yarn start` again: everything should be red! :)

## Reference

Bootstrap Italia documentation is hosted on GitHub pages at https://italia.github.io/bootstrap-italia/docs/come-iniziare/personalizzazione-della-libreria/ (in italian).
