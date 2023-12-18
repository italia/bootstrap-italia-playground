# Bootstrap Italia Playground

This little project is the easiest way to start playing with [Bootstrap Italia](https://italia.github.io/bootstrap-italia/).

<img src="https://github.com/italia/bootstrap-italia-playground/blob/main/.github/bootstrap-italia-playground.png" width="800"> 

## What's included

You'll find a plain HTML page linking Bootstrap Italia files and empty CSS and JS files to enable styling.

```
bootstrap-italia-playground/
│   index.html          # main html file
├── scss/
│   ├── _custom_.scss   # working SCSS file
└── js/
    └── main.js         # working JS file
```

## Getting started

* Install dependencies: `npm install`
* Run a local server: `npm run serve` (auto refresh on every change)
* Point a browser to: `http://127.0.0.1:3000/`

## Updating Bootstrap Italia colours

To update Bootstrap Italia primary colour, please refer to the `scss/_custom.scss` file, where `$primary` colour variable is overridden.  
Just run `npm run serve`: everything should be red! :)

## Changes from Bootstrap Italia version 2.3.0

From [Bootstrap Italia v2.3.0](https://github.com/italia/bootstrap-italia/releases/tag/v2.3.0) we have introduced new semantic variables (linked to the next integration of design tokens).

These variables are:

```scss
$color-background-primary-lighter
$color-text-primary-active
$color-text-primary-hover
```

declared in `_colors_vars.scss` ([from line 392](https://github.com/italia/bootstrap-italia/blob/main/src/scss/utilities/colors_vars.scss)).
Some components now use these variables instead of the old ones (like `$neutral-` or `complementary-`).

To correctly customize the main theme of your BI installation, you must assign a value to the them. You can use HEX, HSL, or HSB values.

## Reference

Bootstrap Italia documentation is hosted on GitHub pages at https://italia.github.io/bootstrap-italia/docs/come-iniziare/personalizzazione-della-libreria/ (in italian).
