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



### 01. fetch 是什么?

 Fetch 是一个新的概念, 等同于 XMLHttpRequest。它提供了许多与XMLHttpRequest相同的功能，但被设计成更具可扩展性和高效性。
 优点:
 1. 语法简洁，更加语义化
 2. 基于标准 Promise 实现，支持 async/await
 3. 同构方便

Fetch API 是基于 Promise 设计，有必要先学习一下 Promise，推荐阅读 [MDN Promise 教程](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

如何使用与详细介绍: [传统 Ajax 指的是 XMLHttpRequest（XHR），未来现在已被 Fetch 替代。](https://github.com/camsong/blog/issues/2)

[fetch API](http://bubkoo.com/2015/05/08/introduction-to-fetch/)

Web'黑话': [Polyfill](https://segmentfault.com/a/1190000002593432#articleHeader1)

---

### 02. promise

Promise 是异步编程的一种解决方案，比传统的解决方案——回调函数和事件——更合理和更强大。它由社区最早提出和实现，ES6 将其写进了语言标准，统一了用法，原生提供了Promise对象。

 特点:
 1. 对象的状态不受外界影响。Promise对象代表一个异步操作，**有三种状态：** Pending（进行中）、Fulfilled（已成功）和Rejected（已失败）。
 2. 一旦状态改变，就不会再变，任何时候都可以得到这个结果。
 
 [ES6阮一峰文档-promise](http://es6.ruanyifeng.com/#docs/promise)

 [mdn promise](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

---

### 03. cookie

HTTP Cookie（也叫Web cookie或者浏览器Cookie）是服务器发送到用户浏览器并保存在浏览器上的一块数据，它会在浏览器下一次发起请求时被携带并发送到服务器上。比较经典的，可以用它来确定两次请求是否来自于同一个浏览器，从而能够确认和保持用户的登录状态。Cookie的使用使得基于无状态的HTTP协议上记录稳定的状态信息成为了可能。

主要用于:
1. 会话状态管理（如用户登录状态、购物车）
2. 个性化设置（如用户自定义设置）
3. 浏览器行为跟踪（如跟踪分析用户行为）

[HTTP Cookies](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies)

---

### 04. nginx

NGINX是一个免费的，轻量级，开源的，高性能的HTTP服务器和反向代理服务器，以及一个IMAP / POP3代理服务器。NGINX以其高性能，稳定性，丰富的功能集，简单的配置和低资源消耗而闻名。

[Nginx 中文官方文档](https://wizardforcel.gitbooks.io/nginx-doc/content/index.html)

[nginx主页](http://nginx.net)

[www.nginx.com](https://www.nginx.com/resources/wiki/)


---


### 05. 跨域

跨域是指从一个域名的网页去请求另一个域名的资源。

跨域的严格一点的定义是：只要 协议，域名，端口有任何一个的不同，就被当作是跨域。 

CORS（Cross-Origin Resource Sharing）跨域资源共享，定义了必须在访问跨域资源时，浏览器与服务器应该如何沟通。CORS背后的基本思想就是使用自定义的HTTP头部让浏览器与服务器进行沟通，从而决定请求或响应是应该成功还是失败。

JSONP（JSON with Padding）是资料格式 JSON 的一种“使用模式”，可以让网页从别的网域要资料。也叫填充式JSON，是应用JSON的一种新方法，只不过是被包含在函数调用中的JSON


[跨域资源共享 CORS 详解](http://www.ruanyifeng.com/blog/2016/04/cors.html)

[详解js跨域问题](https://segmentfault.com/a/1190000000718840)


---

### 06. 优化

1. 请减少HTTP请求

	(1)设置 HTTP缓存

	(2)资源合并与压缩

	(4)精灵图

	(5)多图片网页使用图片懒加载

2. 头部引用css，底部引用js

3. JavaScript 压缩和模块打包 (压缩js css 减少带宽占用)

[网页性能管理详解-阮](http://www.ruanyifeng.com/blog/2015/09/web-page-performance-in-depth.html)

[【译】唯快不破：Web 应用的 13 个优化步骤](https://zhuanlan.zhihu.com/p/21417465?refer=no-backend)

---

### 0.7 打包

1. Webpack
2. gulp
等等~


---

### 08. 线上出bug调试技巧

1. 本地复现、调试、解决、上线
2. 使用 Chrome 浏览器进行 debug
3. 设置 DOM 改变时的断点
4. JS代码格式化
[Chrome 开发者工具](https://developers.google.com/web/tools/chrome-devtools/)

---

### 09. 浏览器缓存

作用:
1. 减少网络带宽消耗
2. 降低服务器压力
3. 减少网络延迟，加快页面打开速度

类型:
1. 服务器端缓存
2. 浏览器端缓存
3. Web应用层缓存
	
[【Web缓存机制系列】](http://www.alloyteam.com/2012/03/web-cache-1-web-cache-overview/)
[浏览器缓存知识小结及应用](https://www.cnblogs.com/lyzg/p/5125934.html)

---

### less和css

[less](http://www.bootcss.com/p/lesscss/)

---

### 11. 前端攻防

1. XSS攻击：跨站脚本攻击(Cross Site Scripting)，为不和 CSS混淆，故将跨站脚本攻击缩写为XSS。
2. CSRF（Cross-site request forgery跨站请求伪造，也被称为“One Click Attack”或者Session Riding，通常缩写为CSRF或者XSRF，是一种对网站的恶意利用。尽管听起来像跨站脚本（XSS）,但它与XSS非常不同，并且攻击方式几乎相左。XSS利用站点内的信任用户，而CSRF则通过伪装来自受信任用户的请求来利用受信任的网站。与XSS攻击相比，CSRF攻击往往不大流行（因此对其进行防范的资源也相当稀少）和难以防范，所以被认为比XSS更具危险性。

[Web前端攻防,一不小心就中招了](https://juejin.im/post/5912740344d904007b010252)

[Web前端攻防](https://zhuanlan.zhihu.com/p/19813739)

---

### 13. options请求和普通的请求有什么不同

单请/普通请求不同，“需预检的请求”要求必须首先使用 OPTIONS   方法发起一个预检请求到服务器，以获知服务器是否允许该实际请求。"预检请求“的使用，可以避免跨域请求对服务器的用户数据产生未预期的影响。

规范要求，对那些可能对服务器数据产生副作用的 HTTP 请求方法（特别是 GET 以外的 HTTP 请求，或者搭配某些 MIME 类型的 POST 请求），浏览器必须首先使用 OPTIONS 方法发起一个预检请求（preflight request），从而获知服务端是否允许该跨域请求。服务器确认允许之后，才发起实际的 HTTP 请求。在预检请求的返回中，服务器端也可以通知客户端，是否需要携带身份凭证（包括 Cookies 和 HTTP 认证相关数据）。


[HTTP访问控制](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Access_control_CORS#概述)

---

### 14. 路由hash和history有什么不同，在不同的浏览器上降级策略。


