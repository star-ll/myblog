#React
# 设计哲学
React 是由 **Facebook（Meta）** 于 2013 年开源的 **革命性 JavaScript 库**，专注于构建用户界面（UI）。它通过 **组件化架构** 与 **声明式编程模型**，彻底改变了开发者构建 Web 应用的方式，使复杂 UI 的开发变得高效、可维护且性能卓越。
React 的诸多创新思想——如**组件化架构**、**单向数据流**、**Hooks 机制**和**虚拟 DOM 模型**——深刻重塑了前端开发范式。深入理解这些设计，不仅能显著提升 React 开发能力，更能帮助开发者洞察现代前端框架的共通设计语言。
总的来说，React 的本质是 **构建可预测 UI 的声明式组件引擎**。它通过 **约束**（单向数据流/不可变性）带来 **自由**（组合扩展/跨平台），通过 **抽象**（虚拟DOM/Hooks）解决 **本质复杂度**（DOM操作/副作用管理）。

# React基本架构
React源码采用Monorepo结构，将不同功能的源代码拆分到不同的子包中，其中有三个包是最常用也是最重要的，即：
- packages/react：包含React核心源码，与环境无关，包括各项API和Hook等。
- packages/scheduler: 包含React调度系统相关源码，负责调度React内部的各项任务。
- packages/react-DOM：包含React将组件转换成DOM相关的源码，负责将（JSX编译后的）ReactElement转化成DOM，从而渲染到屏幕上。
## 核心包
### React
React包是整个React框架的核心，其有多个重要作用：
- 提供相关的TypeScript类型
- 提供Hook，例如useState、useEffect等，供React函数式组件使用
- 提供cache、memo、lazy等API
- 提供Fragment等内置组件
- 提供React.createElement，编译器会将JSX转化成React.createElement函数调用形式来创建ReactElement

### Scheduler


### React-DOM


### 从JSX到Element


### React中的事件系统


## React中的位运算
