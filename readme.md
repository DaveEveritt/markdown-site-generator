# Website for Ecovisum

A rough content plan for the new Ecovisum website, built as a static single page from Markdown files, compiled with [Showdown.js](https://github.com/showdownjs/showdown/wiki/Showdown-options).

## TO DO

- [ ] do mobile menu
- [ ] make design as a skin
- [ ] refactor styles as a neutral wireframe
- [ ] concatenate and minify .js files
- [x] map through an object storing the markdown file paths and HTML destinations
- [x] make Markdown converter generic
- [x] rewrite content (this is a straight copy)
- [x] decide on whether we need a contact form (not yet)

## Minification

leave js/showdown.min.js out

cat js/content.js js/mdconvert.js js/scripts.js > js/scripts.concat.js

uglifyjs doesn't do ES6. Try [Gulp](https://codehangar.io/concatenate-and-minify-javascript-with-gulp/)

or

uglifyjs js/content.js js/mdconvert.js js/scripts.js --compress --mangle --output scripts.min.js

## References

- [answer to "Get text from a txt file in the url"](https://stackoverflow.com/a/39758157/123033)
- [Showdown.js](http://showdownjs.com/)
- [Jake Archibald: "That's so fetch!"](https://jakearchibald.com/2015/thats-so-fetch/)
- MDN: the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) and [Response methods](https://developer.mozilla.org/en-US/docs/Web/API/Response)
- [Sara Vieira: "How to Use the JavaScript Fetch API to Get Data"](https://scotch.io/tutorials/how-to-use-the-javascript-fetch-api-to-get-data)

Also see

- [Remarkable](https://ourcodeworld.com/articles/read/396/how-to-convert-markdown-to-html-in-javascript-using-remarkable)
- [List of Markdown converters](https://stackoverflow.com/questions/1319657/javascript-to-convert-markdown-textile-to-html-and-ideally-back-to-markdown-t/40066280#40066280)
