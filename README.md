css-xpath
====================
[![Build Status](https://travis-ci.org/gburtini/css-xpath.svg?branch=master)](https://travis-ci.org/gburtini/css-xpath) [![Known Vulnerabilities](https://snyk.io/test/github/gburtini/css-xpath/badge.svg)](https://snyk.io/test/github/gburtini/css-xpath) [![npm version](https://badge.fury.io/js/css-xpath.svg)](https://badge.fury.io/js/css-xpath)

Single method library for converting CSS selectors to XPath queries. This forked out of the [Potent Tools](http://github.com/gburtini/Potent-Tools-for-XPath) project, where we are playing archaeologist and recovering some useful but abandoned Firebug code.

Installation
------------
`npm install --save css-xpath`
or
`yarn add css-xpath`

Usage
-----
```js
const cssXPath = require('css-xpath');
cssXPath('html > body') // '//html/body'
```

That's the whole library. Take in a CSS selector, output an XPath query. 

They're unexposed, but if you want, there's some [regular expressions](src/patterns.js) that might be interesting if you're trying to parse CSS yourself. They are not exposed, 

License
-------

As the code in this repository is derived from the Firebug source code, its [BSD 3-clause license](https://github.com/firebug/firebug/blob/master/extension/license.txt) applies.

