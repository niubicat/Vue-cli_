**************************
Vue 全家桶：
**************************

## Vue

#### assets 和 static 区别
* assets放置的是组件的资源，static放置的是非组件的资源
* 比如说即static下的文件资源作为src路径传入组件中，文件的path是可以被解析了，而assets则不行
* 比如你写一个音乐播放器，类似的播放键和上一曲下一曲这些图标就应该作为组件资源放在assests里面，
* 而不同音乐选集的封面这些是应该作为文件资源放在static下

### 一、管理目录

#### src

* api: 后端api接口
* assets: 组件的资源
* directive 自定义指令
* filter 自定过滤指令
* mock 模拟借口数据
* router 路由设置
* store 状态管理
* style 样式文件
* utils 公共方法
* vendor 第三方库
* views 页面

## Vuex

### 一、store

#### modules 状态模块(vue中包含有多个状态模块)
count moduleA = {
    state: {},
    mutations: {}, // mutations 改变store状态的唯一方法，相当于react中的reducer方法
    actions：{},
    getters: {}
}

* 例如：permission.js 自定义路由权限状态模块




