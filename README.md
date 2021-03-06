hexo-codepen [![NPM version][npm-image]][npm-url] [![Dependency Status][depstat-image]][depstat-url]
================

A better version of [hexo-tag-codepen][hexo-tag-codepen-link] with a valid HTML.

> [Hexo] tag to embed code snippet from [CodePen]

## Install

Install using [npm][npm-url].

    $ npm install hexo-codepen --save

or using [yarn][yarn-url]

    $ yarn add hexo-codepen

## Usage

Create [Embedded Pen] with following syntax:

```
  {% codepen userId|anonymous|anon slugHash theme [defaultTab [height [width]]] %}
```
## How to get arguments from CodePen embed

This is something generated by `CodePen`:
```html
<p data-height="265" data-theme-id="dark" data-slug-hash="bgjKKE" data-default-tab="css,result" data-user="CiTA" data-embed-version="2" data-pen-title="CSS sidebar toggle" class="codepen">See the Pen <a href="https://codepen.io/CiTA/pen/bgjKKE/">CSS sidebar toggle</a> by Silvestar Bistrović (<a href="https://codepen.io/CiTA">@CiTA</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>
```
You can extract required arguments:

Field      | Value
-----------|--------
userId     | CiTA  
slugHash   | bgjKKE  
theme      | dark  
defaultTab | css,result  
height     | 265  
width      | This value should be adjusted according to your blog theme, by default it is `100%`

## License
MIT

[![NPM downloads][npm-downloads]][npm-url]

[homepage]: https://github.com/maliMirkec/hexo-tag-codepen
[hexo-tag-codepen-link]: https://github.com/maliMirkec/hexo-tag-codepen

[npm-url]: https://npmjs.org/package/hexo-codepen
[npm-image]: http://img.shields.io/npm/v/hexo-codepen.svg?style=flat
[npm-downloads]: http://img.shields.io/npm/dm/hexo-codepen.svg?style=flat

[yarn-url]: https://yarnpkg.com/en/package/hexo-codepen

[depstat-url]: https://gemnasium.com/maliMirkec/hexo-tag-codepen
[depstat-image]: http://img.shields.io/gemnasium/maliMirkec/hexo-tag-codepen.svg?style=flat

[Hexo]: http://hexo.io/
[CodePen]: http://codepen.io/
[Embedded Pen]: http://blog.codepen.io/documentation/features/embedded-pens/
