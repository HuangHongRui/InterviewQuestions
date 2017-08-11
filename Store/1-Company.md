# 面试题

01. fetch
02. promise
03. cookie
04. nginx
05. 跨域
06. 优化
07. 打包
08. 线上出bug调试技巧
09. 浏览器缓存
10. less和css
11. 前端攻防
12. css面试
13. options请求和普通的请求有什么不同
14. 路由hash和history有什么不同，在不同的浏览器上降级策略。


---



### 1. fetch 是什么?

 Fetch 是一个新的概念, 等同于 XMLHttpRequest。它提供了许多与XMLHttpRequest相同的功能，但被设计成更具可扩展性和高效性。
 优点:
 1. 语法简洁，更加语义化
 2. 基于标准 Promise 实现，支持 async/await
 3. 同构方便

Fetch API 是基于 Promise 设计，有必要先学习一下 Promise，推荐阅读 [MDN Promise 教程](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

如何使用与详细介绍: [传统 Ajax 指的是 XMLHttpRequest（XHR），未来现在已被 Fetch 替代。](https://github.com/camsong/blog/issues/2)

[fetch API](http://bubkoo.com/2015/05/08/introduction-to-fetch/)

Web'黑话': [Polyfill](https://segmentfault.com/a/1190000002593432#articleHeader1)



### 2. promise

Promise 是异步编程的一种解决方案，比传统的解决方案——回调函数和事件——更合理和更强大。它由社区最早提出和实现，ES6 将其写进了语言标准，统一了用法，原生提供了Promise对象。

 特点:
 1. 对象的状态不受外界影响。Promise对象代表一个异步操作，**有三种状态：** Pending（进行中）、Fulfilled（已成功）和Rejected（已失败）。
 2. 一旦状态改变，就不会再变，任何时候都可以得到这个结果。
 
 [ES6阮一峰文档-promise](http://es6.ruanyifeng.com/#docs/promise)
 [mdn promise](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

