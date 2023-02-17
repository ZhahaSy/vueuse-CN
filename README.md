<p align="center">
<a href="https://github.com/vueuse/vueuse#gh-light-mode-only">
  <img src="https://raw.githubusercontent.com/vueuse/vueuse/main/packages/public/logo-vertical.png#gh-light-mode-only" alt="VueUse - Collection of essential Vue Composition Utilities" width="300">
</a>
<a href="https://github.com/vueuse/vueuse#gh-dark-mode-only">
  <img src="https://raw.githubusercontent.com/vueuse/vueuse/main/packages/public/logo-vertical-dark.png#gh-dark-mode-only" alt="VueUse - Collection of essential Vue Composition Utilities" width="300">
</a>
<br>
基本的 Vue 组合utils 集合
</p>

<p align="center">
<a href="https://www.npmjs.com/package/@vueuse/core" target="__blank"><img src="https://img.shields.io/npm/v/@vueuse/core?color=a1b858&label=" alt="NPM version"></a>
<a href="https://www.npmjs.com/package/@vueuse/core" target="__blank"><img alt="NPM Downloads" src="https://img.shields.io/npm/dm/@vueuse/core?color=50a36f&label="></a>
<a href="https://vueuse.org" target="__blank"><img src="https://img.shields.io/static/v1?label=&message=docs%20%26%20demos&color=1e8a7a" alt="Docs & Demos"></a>
<img alt="Function Count" src="https://vueuse.org/badge-function-count.svg">
<br>
<a href="https://github.com/vueuse/vueuse" target="__blank"><img alt="GitHub stars" src="https://img.shields.io/github/stars/vueuse/vueuse?style=social"></a>
</p>

<p align="center">
  <a href="https://cdn.jsdelivr.net/gh/antfu/static/sponsors.svg">
    <img src='https://cdn.jsdelivr.net/gh/antfu/static/sponsors.svg'>
  </a>
</p>

## 🚀 特点

- 🎪 [**交互式文档 & demos**](https://vueuse.org)
- 🕶 **无缝切换**:  Vue 3 和 2  **都可以** 使用
- ⚡ **支持 tree shaking**: 只会打包使用到的Util, [utils大小 列表](https://vueuse.org/export-size)
- 🦾 **强类型**: 使用 [TypeScript](https://www.typescriptlang.org/) 编写, 以及ts注释 [TS Docs](https://github.com/microsoft/tsdoc)
- 🔋 **友好的 SSR**
- 🌎 **支持外链**: 可通过CDN使用
<!-- @TODO 待确认 原文：Configurable event filters and targets -->
- 🔩 **更灵活**: 可配置的事件过滤器和目标
- 🔌 **可选 [附件](https://vueuse.org/add-ons)**: Router, Firebase, RxJS, etc.

## 🦄 用法

```ts
import { useLocalStorage, useMouse, usePreferredDark } from '@vueuse/core'

export default {
  setup() {
    // 记录鼠标位置
    const { x, y } = useMouse()

    // 改变网页主题色为黑暗模式
    const isDark = usePreferredDark()

    // 响应式的 localStorage
    const store = useLocalStorage(
      'my-storage',
      {
        name: 'Apple',
        color: 'red',
      },
    )

    return { x, y, isDark, store }
  },
}
```

详情参考 [函数列表](https://vueuse.org/functions) 或 [文档](https://vueuse.org/).

## 📦 安装

> 🎩 从v4.0开始, 使用[vue-demi](https://github.com/vueuse/vue-demi)，使其可以**同时支持**vue2和vue3

```bash
npm i @vueuse/core
```

[Add ons](https://vueuse.org/add-ons.html) | [Nuxt Module](https://vueuse.org/guide/index.html#nuxt)

> 从v4.0开始, VueUse 要求 `vue` >= v3.2 or `@vue/composition-api` >= v1.1

###### Demos

- [Vite + Vue 3](https://github.com/vueuse/vueuse-vite-starter)
- [Nuxt 3 + Vue 3](https://github.com/antfu/vitesse-nuxt3)
- [Webpack + Vue 3](https://github.com/vueuse/vueuse-vue3-example)
- [Nuxt 2 + Vue 2](https://github.com/antfu/vitesse-nuxt-bridge)
- [Vue CLI + Vue 2](https://github.com/vueuse/vueuse-vue2-example)

### CDN

```html
<script src="https://unpkg.com/@vueuse/shared"></script>
<script src="https://unpkg.com/@vueuse/core"></script>
```

会在全局暴露出来，使用 `window.VueUse` 获取

## 🪴 项目活跃度

![Alt](https://repobeats.axiom.co/api/embed/a406ba7461a6a087dbdb14d4395046c948d44c51.svg "Repobeats分析图像")

## 🧱 贡献

请查收 [**贡献指南**](https://vueuse.org/contributing)

## 🌸 鸣谢

本项目是收到一下项目的启发和参考

- [streamich/react-use](https://github.com/streamich/react-use)
- [u3u/vue-hooks](https://github.com/u3u/vue-hooks)
- [logaretm/vue-use-web](https://github.com/logaretm/vue-use-web)
- [kripod/react-hooks](https://github.com/kripod/react-hooks)

同时感谢 [贡献代码的所有的contributor](https://github.com/vueuse/vueuse/graphs/contributors)!

## 👨‍🚀 Contributors

### Financial Contributors on Open Collective

<a href="https://opencollective.com/vueuse"><img src="https://opencollective.com/vueuse/individuals.svg?width=890"></a>

## 📄 License

[MIT License](https://github.com/vueuse/vueuse/blob/main/LICENSE) © 2019-PRESENT [Anthony Fu](https://github.com/antfu)
