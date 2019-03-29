# vuex-router

> A Vue.js project

---

## 開発手順

### Vue-CLIをグローバルインストール

```
$ npm i -g vue-cli
```

### プロジェクト作成

```
$ vue init webpack-simple <PROJECT_NAME>
$ cd <PROJECT_NAME>
$ npm i
```

### 立ち上げ

```
$ npm run dev
```

### Vue-Routerをインストール

```
$ npm i -S vue-router
```

### Vue-Routerのセッティング

```
import Vue from 'vue';
import VueRouter from 'vue-router';    // VueRouterをインポート
import App from './App.vue';
import { routes } from './routes';    // routes.jsをインポート(ルート情報を書き込むファイル)

Vue.use(VueRouter);    // VueRouterをVueのミドルウェアとして使用する宣言

const router = new VueRouter({
  routes
});    // routes.jsの情報をVueRouterに入れる

new Vue({
  el: '#app',
  router,    // Vueをインスタンス化する際にrouterを渡す
  render: h => h(App)
})
```

---

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
