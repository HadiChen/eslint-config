# eslint-config

## 简介

`eslint`配置。

配置分为 `basic`、 `typescript`、 `vue`、 `react` `4`个模块，分别对应场景：

1. `basic` -- 纯js开发。
2. `typescript` -- typescript开发，继承`basic`，如`nodejs`等。
3. `vue` -- vue项目开发，继承`typescript`。
4. `react` -- react项目开发，继承`typescript`。

## 安装

```ts
npm install eslint @hdchan/eslint-config --save-dev
// or
yarn add eslint @hdchan/eslint-config -D
```

## 配置文件`.eslintrc.js`

```ts
// vue 项目使用
module.exports = {
  root: true,
  extends: [
    '@hdchan/eslint-config/vue',
  ],
};

// js 项目使用
module.exports = {
  root: true,
  extends: [
    '@hdchan/eslint-config/basic',
  ],
};

// typescript 项目使用
module.exports = {
  root: true,
  extends: [
    '@hdchan/eslint-config/typescript',
  ],
};

// react 项目使用
module.exports = {
  root: true,
  extends: [
    '@hdchan/eslint-config/react',
  ],
};
```
