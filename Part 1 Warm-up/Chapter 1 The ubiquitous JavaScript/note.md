# 第1章 无处不在的JavaScript

本章包括的内容

- JavaScript核心语言特性
- JavaScript引擎核心要素
- JavaScript开发中的3个最佳实践
  
Node、ApacheCordova、Electron

## 1.1 “理解”JavaScript语言

与其他主流语言相比，JavaScript函数式语言的血统更多一些。JavaScript中的一些概念从根本上不同于其他的语言。

这些根本性的差异包括以下内容

- 函数是一等公民（一级对象）———— 在JavaScript中,函数与其他对象共存，并且能够像任何其他对象一样地使用。函数可以通过字面量创建，可以赋值给变量，可以作为函数参数进行传递，甚至可以作为返回值从函数中返回。
- 函数闭包 ———— **当函数主动维护了在函数内部使用的外部变量，则该函数为一个闭包。**
- 作用域 ————
- 基于原型的面向对象

对象、原型、函数和闭包的紧密结合组成了JavaScript

其他的一些功能，帮助书写优雅高效的代码。

- 生成器 一种可以基于一次请求生成多次值的函数，在不同请求之间也能挂起执行。
- Promise，让我们更好地控制异步代码。
- 代理，让我们控制对特定对象的访问。
- 高级数组方法，书写更优雅的数组处理函数。
- Map，用于创建字典集合；Set，处理仅包含不重复项目的集合。
- 正则表达式，简化用代码书写起来很复杂的逻辑。
- 模块，把代码划分为较小的可以自包含的片段，使项目易于管理。

### 1.1.1 JavaScript是如何发展的

<https://kangax.github.io>

### 1.1.2 如今的转换编译器已经能让我们体验未来的JavaScript

当我们想利用JavaScript的最新特性时，也往往会被残酷的现实绑架：用户依然在使用老旧的浏览器。

解决这个问题的方式之一时使用转换编译器transpilers（即“转换器+编译器”，“transformation + compiling”），这类工具能够把最前沿的JavaScript代码转换为等价的（如果不能实现，则使用相似的）能在当前浏览器中运行的代码。

最流行的转换编译器时Traceur和Babel。

<https://github.com/googLe/traceur-compiler/wiki/Getting-stanted>
<https://github.com/google/traceur-compiler>
<http://babeljs.io/docs/setup>

[Babel中文](https://www.babeljs.cn/)

## 1.2 理解浏览器

JavaScript最初的运行环境是浏览器环境，而其他运行环境也是借鉴与浏览器环境。我们重点专注浏览器环境。浏览器提供了多种概念和API让我们探索，如图1.1 ![1.1](./1.1.png)**我们将集中讨论如下概念**

- 文档对象模型
