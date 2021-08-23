# Vue3.0 learning...

-   api 介绍
-   原理介绍（原理不是源码！！！）

## 关于 vue3.0 总结问题如下

### `vue3` 比 `vue2` 有什么优势

-   性能更好
-   体积更小(仅限于基于 vue2 的体积更加优化)
-   更好的 ts 支持
-   更好的代码组织
-   更好的逻辑抽离
-   更多新功能

### 描述 vue3 `生命周期`

-   LifeCycles.vue 文件
-   Options AP 生命周期
    -   1. beforeDestory 改为 beforeUnmount
    -   2. destory 改为 unmounted
    -   3. 其他沿用 vue2 的生命周期
-   Composition API 生命周期

### 如何看待 `Composition API` 和 `Options API`

-   Composition API(组合式 api)
    -   1. 在官方文档不属于基础用法属于高阶技巧
    -   2. 为了解决复杂业务逻辑而设计的
    -   3. 类似于 Hooks 在 React 中的地位
-   Composition API 带来了什么
    -   1. 针对大型复杂项目来说 更好的代码组织
    -   2. 逻辑复用(后续会有代码演示)
    -   3. 类型推导(vue2.0 的 this 语法不利于正常 js 语法的类型推导)
-   如何选择：
    -   1. 不建议混用,写法、代码组织复用方式，会引起混乱
    -   2. 简单项目采用维护成本低的 Options API

### 如何理解 `ref` `toRef` `toRefs`

-   ref 生成值类型的响应式数据 可用于模板和 reactive 通过.value 修改值 获取模板内的 dom 元素
-   toRef 针对一个响应式对象(reactive)的 prop 创建一个 ref 具有响应式 两者保持引用关系

### vue3 升级了哪些重要的功能

### `Composition API` 如何实现代码逻辑复用

### vue3 如何实现 `响应式`以及 `模板编译`

### `watch` 和 `watchEffect` 的区别是什么

### `setup` 中如何获取组件实例

### vue3 为何比 vue2 快

### `vite` 是什么

### `Composition API` 和 `React Hooks` 的对比
