# vue-social-share

> A Vue 2.x social share component based on [Share.js](https://github.com/overtrue/share.js)

[![NPM version](https://img.shields.io/npm/v/vue-social-share.svg?style=flat)](https://npmjs.com/package/vue-social-share)
[![Vue 2.x](https://img.shields.io/badge/Vue-2.x-brightgreen.svg)](https://vuejs.org/v2/guide/)
[![NPM downloads](https://img.shields.io/npm/dm/vue-social-share.svg?style=flat)](https://npmjs.com/package/vue-social-share)

[Live Demo](http://vue-social-share.surge.sh/)

## Install

```bash
npm install vue-social-share -S
```

## Usage

```js
import Vue from 'vue'
import Share from 'vue-social-share'

Vue.use(Share)

<share :config="config"></share>
```

## Props

props `config` 是一个对象，包含如下属性。

```
url                 : '', // 网址，默认使用 window.location.href
source              : '', // 来源（QQ空间会用到）, 默认读取head标签：<meta name="site" content="http://overtrue" />
title               : '', // 标题，默认读取 document.title 或者 <meta name="title" content="share.js" />
description         : '', // 描述, 默认读取head标签：<meta name="description" content="PHP弱类型的实现原理分析" />
image               : '', // 图片, 默认取网页中第一个img标签
sites               : ['qzone', 'qq', 'weibo','wechat', 'douban'], // 启用的站点
disabled            : ['google', 'facebook', 'twitter'], // 禁用的站点
wechatQrcodeTitle   : '微信扫一扫：分享', // 微信二维码提示文字
wechatQrcodeHelper  : '<p>微信里点“发现”，扫一下</p><p>二维码便可将本文分享至朋友圈。</p>'
```

## 支持站点

微博、QQ 空间、QQ 好友、微信、腾讯微博、豆瓣、Facebook、Twitter、Linkedin、Google+

## Development

- `yarn example`: Run example in development mode
- `yarn build`: Build component in both format

## Credits

- [Share.js](https://github.com/overtrue/share.js)

# License

This content is released under the [MIT](http://opensource.org/licenses/MIT) License.
