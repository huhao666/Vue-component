# Vue 组件与组件化

## 从 JQuery 到组件化需要关注的几个问题

- 怎么去理解组件？
- 为什么要组件化？
- 平时的开发与组件化开发最显著的区别是什么？
- 怎么去理解数据驱动？

## 组件化开发要具备的知识

### 组件的分类

- 基础组件
- 页面组件
- 业务组件

### 组件间的通信方式

#### 组件之间的三种关系

- 父子
- 祖孙
- 兄弟

#### 三个重要的 API

- props
- event
- slot

#### 内置的通信手段

- `ref`
- `$parent`/`$children`

#### 跨组件通信

- provide / inject (Vue.js 2.2.0 以后新增的)
  不建议在业务组件中使用
  主要用于组件库中的联动关系的组件
- dispatch / broadcast (事件)
- findComponents (拿到组件实例)
- eventBus
- vuex

## 怎么合理的拆分组件

解耦组件的交互逻辑，尽量把复杂的逻辑分发到不同的子组件中