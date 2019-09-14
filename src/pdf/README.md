# Parsing the refactoring pdf
This script parses the refactoring 2nd edition pdf and exports as text file.

## Getting started
```
npm install
```

after installed change into the refactoring directory
```
cd refactoring
```

run the script
```
node parse-refactoring.js
```

The output of the script will be under `assets/`

## Resources
- [pdfjs](https://mozilla.github.io/pdf.js/)
- [pdf-parse](https://www.npmjs.com/package/pdf-parse)
- pdfjs examples
  - [getinfo](https://github.com/mozilla/pdf.js/blob/master/examples/node/getinfo.js)
  - [api source](https://github.com/mozilla/pdf.js/blob/master/src/display/api.js)
- [pdf.js/issues/8599](https://github.com/mozilla/pdf.js/issues/8599)
- [Extract text in the right order](https://stackoverflow.com/questions/50788543/pdf-js-mozilla-lib-issue-get-or-extract-pure-text-with-right-order)

## Notes & Assumptions
- `src/pdf/assets/refactoring-improving-existing-2nd.pdf` exists.
- x, y positions of text in pdf.js, maps to `transform[4]` and `transform[5]`
