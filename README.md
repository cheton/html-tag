# html-tag [![build status](https://travis-ci.org/cheton/html-tag.svg?branch=master)](https://travis-ci.org/cheton/html-tag) [![Coverage Status](https://coveralls.io/repos/cheton/html-tag/badge.svg)](https://coveralls.io/r/cheton/html-tag)
[![NPM](https://nodei.co/npm/html-tagjs.png?downloads=true&stars=true)](https://nodei.co/npm/html-tagjs/)

A simple utility for creating HTML tags.

## Installation

```bash
npm install --save html-tagjs
```

## Usage
```js
import tag from 'html-tagjs';

tag('a', { href: 'http://example.com' }, 'Example');
// → '<a href="http://example.com">Example</a>'

tag('input', { name: 'name', value: 'Input your name...' });
// → '<input name="name" value="Input your name..."/>'

tag('div', { title: '\'"&<>' }, tag('i', { class: 'icon icon-folder' }, ''));
// → '<div title="&#39;&quot;&amp;&lt;&gt;"><i class="icon icon-folder"></i></div>'
```

## License

Copyright (c) 2016 Cheton Wu

Licensed under the [MIT License](LICENSE).