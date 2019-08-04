# travel

> A mobile web project on Vue.js  

## demo地址：https://tedqin.github.io/Travel/

## 仿某旅游网站的移动端webapp页面
## 启动

``` bash
# 安装依赖
npm install

# 本地端口启动
npm run start

# 打包
npm run build
```

## 组件
* home 
	* Header 头部 
	* Icon 原型图标区域 
	* Recommend 推荐 
	* Swiper 图片轮播 
	* Weekend 周末推荐
* city 
	* Header 头部 
	* Alphabet 右侧城市首字母下拉列表 
	* List 城市列表 
	* Search 搜索
* detail 
	* Header 头部 
	* Banner 主页面 
	* List 图片详情页的轮播

## 用到的功能和插件
* webpack
* axios 发送ajax请求
* vue-awesome-swiper 轮播图插件
* betterscroll 滚动插件，贴近真实的移动端手指滑动
* vuex 进行home和city页面的数据交互，在city页面选择城市，home页面的城市会改变，并且使用router.push自动跳转到home页面
* localstorage 自动缓存，刷新页面的时候已经选择的城市不发生改变
* keepalive 优化问题：防止切换页面会发生多次ajax请求
* 异步组件加载：按需加载组件
