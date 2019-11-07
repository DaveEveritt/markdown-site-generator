# Website generated from separate markdown files


page built from Markdown files compiled with [Showdown.js](https://github.com/showdownjs/showdown/wiki/Showdown-options). Just edit the markdown, push and the live site is updated.

## TO DO

- [ ] put `pages` in a more flexible data structure
- [ ] replace EcoVisum material
- [ ] contain code in an IIFE
- [ ] do mobile menu
- [ ] make design as a skin
- [ ] refactor styles as a neutral wireframe
- [ ] automate minification of .js files
- [X] add "use strict"

## Minification

leave js/showdown.min.js out

cat js/content.js js/mdconvert.js js/scripts.js > js/scripts.concat.js

uglifyjs doesn't do ES6. Try one of these:

- [Douglas Crockford's JSMin](http://www.crockford.com/javascript/jsmin.html)
- [Terser](https://github.com/terser-js/terser/blob/master/README.md)

or go with the herd and try [Gulp](https://codehangar.io/concatenate-and-minify-javascript-with-gulp/)

## JavaScript linting and formatting

use the Prettier and Healthier modules, which can be installed globally.

In package.json:

    "lint": "healthier && prettier --check '**/*.{js,json,css,yml}'",
    "format": "prettier --write '**/*.{js,json,css,yml}'"

## References

- Test: free hosting etc. from GitHub to Render.com: [ecovisum.onrender.com](https://ecovisum.onrender.com/)
- [answer to "Get text from a txt file in the url"](https://stackoverflow.com/a/39758157/123033)
- [Showdown.js](http://showdownjs.com/)
- [Jake Archibald: "That's so fetch!"](https://jakearchibald.com/2015/thats-so-fetch/)
- MDN: the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) and [Response methods](https://developer.mozilla.org/en-US/docs/Web/API/Response)
- [Sara Vieira: "How to Use the JavaScript Fetch API to Get Data"](https://scotch.io/tutorials/how-to-use-the-javascript-fetch-api-to-get-data)

Also see

- [Remarkable](https://ourcodeworld.com/articles/read/396/how-to-convert-markdown-to-html-in-javascript-using-remarkable)
- [List of Markdown converters](https://stackoverflow.com/questions/1319657/javascript-to-convert-markdown-textile-to-html-and-ideally-back-to-markdown-t/40066280#40066280)
