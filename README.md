# Whay
A terminal Eng-Chn dictionary.

终端英文词典

词典使用的有道, 直接使用的web接口, 这下不担心api被限的问题.

# 安装

```shell
npm install -g whay
//或者
yarn global add whay
```

# 使用

```shell
whay my-word

whay --help
```

# Api

```javascript
const whay = require('whay').translate

whay('WordToTranslate', (err, translatedData) => {
  if (err) return
  console.log(translatedData)
})

// translatedData schema
{ keyword: 'WordToTranslate',
  phonetic: '[...]',
  trans: [ '...', '...', ... ]
}
```

# License

MIT
