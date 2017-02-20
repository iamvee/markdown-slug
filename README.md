## Usage

```js
var slugify = require('markdown-slug');

// forward slashes
console.log(slugify('Some/Article'));
//=> 'somearticle'

// backticks
console.log(slugify('Some`Article`'));
//=> 'somearticle'

// CJK punctuations
console.log(slugify('存在，【中文】；《标点》、符号！的标题？'));
//=> '%E5%AD%98%E5%9C%A8%E4%B8%AD%E6%96%87%E6%A0%87%E7%82%B9%E7%AC%A6%E5%8F%B7%E7%9A%84%E6%A0%87%E9%A2%98'

// &
console.log(slugify('Foo & Bar'));
//=> 'foo--bar'
```

