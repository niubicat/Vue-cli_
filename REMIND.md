[*vue-element-admin*](https://github.com/PanJiaChen/vue-element-admin/blob/master/src/store/modules/permission.js)
[*登录权限篇*](https://juejin.im/post/591aa14f570c35006961acac)

**************************
Vue 全家桶：vue(页面), vue-router(路由), vuex(状态管理), vue-resource/axios(异步action), vue-cli(构建工具)
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

### 二、tore

#### modules 状态模块(vue中包含有多个状态模块)


 * @states: 单一全局状态和局部状态
 * @mutations: 改变store状态的唯一方法，相当于react中的reducer方法,每一个 mutation 执行完成后都可以对应到一个新的状态（和 reducer 一样）
 * @actions: mutation 像事件注册，需要相应的触发条件。而 Action 就那个管理触发条件的, Action 提交的是 mutation，而不是直接变更状态
 * @getters: 多组件都使用这个状态，抽象出来共享，暴露为store.getters对象


count moduleA = {
    state: {},
    mutations: {},
    actions：{},
    getters: {}
}

* 例如：permission.js 自定义路由权限状态模块

### 三、组件/模版template

* @mapGetters: 辅助函数仅仅是将store中的getters映射到局部计算属性中，用法和mapState类似






