# travel

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## 组件
home header头部 icon原型图标区域 recommend推荐 swiper图片轮播 weekend周末去哪
city header头部 alphabet:右侧城市首字母下拉列表 list:城市列表 search：搜索
detail
## 响应式
## webpack
## swiper 轮播图
## betterscroll
## vuex 进行home和city页面的数据交互，在city页面选择城市，home页面的城市会改变，并且使用router.push自动跳转到home
## localstorage  刷新的时候选择的城市不变
## keepalive 优化问题：切换页面会发生多次ajax请求