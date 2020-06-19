# Tailwind Mix

This extension provides instant Tailwindcss support to Laravel Mix builds.

## Usage

First, install the extension.

```
npm install tailwind-mix --save-dev
```

Then, require it within your `webpack.mix.js` file, like so:

```js
let mix = require('laravel-mix');

require('tailwind-mix');

mix
    .js('resources/js/app.js', 'public/js')
    .sass('resources/sass/app.scss', 'public/css')
    .tailwind();
```

## Next steps

This package requires tailwind configuration (tailwind.js or tailwind.config.js), so don't forget to run:

```
npx tailwindcss init
npm run dev
```

app.scss file example:

```
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```


And you're done! Compile everything down with `npm run dev`

[More information about the Tailwind directives](https://tailwindcss.com/docs/installation#2-add-tailwind-to-your-css) to your Sass/Less/Stylus entry file.)
