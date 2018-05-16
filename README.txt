// 
Reference1: React中文网 -- https://doc.react-china.org/
Reference2: React官方网站 -- https://reactjs.org/docs/rendering-elements.html
Reference3: 在线Babel编译器 -- https://babeljs.io/repl/#?babili=false&evaluate=true&lineWrap=false&presets=es2015%2Creact%2Cstage-0&code=function%20hello()%20%7B%0A%20%20return%20%3Cdiv%3EHello%20world!%3C%2Fdiv%3E%3B%0A%7D


// Chapter0 -- HelloWorld

// Chapter1 -- JSX 简介
Q: 什么叫JSX？
A: 一种 JavaScript 的语法扩展。比如: const element = <h1>Hello, world!</h1>;

Q: 什么叫JavaScript表达式？
A: An expression is any valid unit of code that resolves to a value.

Q: 如何在 JSX 中使用表达式？
A: 可以任意地在 JSX 当中使用 JavaScript 表达式，在 JSX 当中的表达式要包含在大括号里。

Q: 设置JSX 属性有哪些方式？
A:
1. 可以使用引号来定义以字符串为值的属性;
2. 也可以使用大括号来定义以 JavaScript 表达式为值的属性;


// Chapter2 -- 元素渲染
Q: 什么是React元素？
A: 元素是构成 React 应用的最小单位。

Q: React元素和浏览器的 DOM 元素有什么区别？
A: React元素与浏览器的 DOM 元素不同，React 当中的元素事实上是普通的对象，
React DOM 可以确保 浏览器 DOM 的数据内容与 React 元素保持一致。

Q: 如何更新元素渲染？
A: 由于React元素是immutable 不可变的，当元素被创建之后，你是无法改变其内容或属性的。
一个元素就好像是动画里的一帧，它代表应用界面在某一时间点的样子。

Q: React是如何更新元素的？
A: React 只会更新必要的部分，React DOM 首先会比较元素内容先后的不同，而在渲染过程中只会更新改变了的部分。

// Chapter3 -- 组件 & Props
Q: 什么叫组件?
A: 组件从概念上看就像是函数，它可以接收任意的输入值（称之为“props”），
并返回一个需要在页面上展示的React元素。

Q: 定义组件的方式有哪些？
A: 1.函数定义。定义一个组件最简单的方式是使用JavaScript函数。
2.类定义组件。你也可以使用 ES6 class 来定义一个组件。

Q: 组件名称必须以大写字母开头吗?
A: 是的。React元素可以是DOM标签，也可以是用户自定义的组件。
例如，<div /> 表示一个DOM标签，但 <Welcome /> 表示一个组件，并且在使用该组件时你必须定义或引入它。

Q: 什么叫组合组件？
A: 组件可以在它的输出中引用其它组件，这就可以让我们用同一组件来抽象出任意层次的细节。
在React应用中，按钮、表单、对话框、整个屏幕的内容等，这些通常都被表示为组件。

Q: 什么叫有状态的组件？
A: 能根据当前的状态来渲染UI的组件。

Q: 什么叫"纯函数"？
A: 纯函数是指不依赖于且不改变它作用域之外的变量状态的函数。

Q: React中props有哪些特性？
A: props是只读的，无论是使用函数或是类来声明一个组件，它决不能修改它自己的props。


// Chapter4 -- State & 生命周期
Q: 当React组件被挂载和卸载时会调用什么函数？
A：componentDidMount和componentWillUnmount，这些方法被称作生命周期钩子。

Q: 什么叫"数据自顶向下流动"？
A: 

// Chapter5 -- 事件处理
Q: React 元素的事件处理和 DOM元素的很相似。但在语法上有哪一点不同？
A:
1. React事件绑定属性的命名采用驼峰式写法，而不是小写。
2. 如果采用 JSX 的语法你需要传入一个函数作为事件处理函数，而不是一个字符串(DOM元素的写法)

// Chapter6 -- 条件渲染
Q: 什么叫条件渲染？
A: 在 React 中，你可以创建不同的组件来封装各种你需要的行为。
然后还可以根据应用的状态变化只渲染其中的一部分。

// Chapter7 -- 列表 & keys


// Chapter8 -- 表单


// Chapter9 -- 状态提升
Q: 什么叫状态提升？
A: 使用 react 经常会遇到几个组件需要共用状态数据的情况。
这种情况下，我们最好将这部分共享的状态提升至他们最近的父组件当中进行管理。

Q: "状态提升"对比"双向绑定"有哪些优缺点？
A: 状态提升比双向绑定方式要写更多的“模版代码”，但带来的好处是，你也可以更快地寻找和定位bug的工作。因为哪个组件保有状态数据，也只有它自己能够操作这些数据，发生bug的范围就被大大地减小了。此外，你也可以使用自定义逻辑来拒绝或者更改用户的输入。

// Chapter10 -- 组合 vs. 继承


// Chapter11 -- React理念
Q: React 最初的目的是什么？
A: 使用 JavaScript 创建大型的，快速响应的网络应用




































