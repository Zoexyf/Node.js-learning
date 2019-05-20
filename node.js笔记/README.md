# Node.js 第1天



## 准备知识

### MDN

[MDN](https://developer.mozilla.org/zh-CN/)

### 浏览器工作原理

1. 浏览器组成
2. 浏览器渲染引擎工作原理
3. 通过浏览器访问网站全过程

### Web 开发本质

1. 请求: 客户端发起请求.
2. 处理: 服务器 处理请求.
3. 响应: 服务器将处理结果发送给客户端.

Web应用程序与桌面应用程序对比（计算器案例）

关于C/S（Client/Server） 和 B/S（Browser/Server）

![Client / Server](C:/Users/ZOE%20XU/Desktop/node.js%E7%AC%94%E8%AE%B0/01-%E7%AC%94%E8%AE%B0%E5%A4%A7%E7%BA%B2/imgs/client-server.png)







## Node.js介绍

### 为什么要学习Node.js

企业需求

- 具有服务端开发经验更好
- front-end
- back-end
- 全栈开发工程师（全干）

基本的网站开发功能

- 服务端 
- 前端 
- 运维部署 

多人社区





![](C:/Users/ZOE%20XU/Desktop/node.js%E7%AC%94%E8%AE%B0/images/%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%BB%91%E7%9B%92%E5%AD%90.png)



- ### Node.js 是什么

  Node.js® is a JavaScript runtime built on [Chrome's V8 JavaScript engine](https://v8.dev/).

  Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行环境。 (代码是字符串，引擎解析和执行)

  Node.js 使用了一个事件驱动、非阻塞式 I/O 的模型（异步操作），使其轻量又高效。

  npm是世界上最大的开源生态系统，绝大多数的JavaScript相关的包都存放在了npm上，这样做的目的是为了让开发人员更方便的去下载使用 

  ```
  npm install jquery
  ```

  + Node.js不是一门语言、不是库、不是框架
  + Node.js是一个JavaScript运行时的环境----也就是Node.js可以解析和执行JavaScript代码
  + 之前只有浏览器可以解析，现在JavaScript可以完全脱离浏览器来运行：Node.js

-   浏览器中的JavaScript

  + EcmaScript
    + 基本的语法
    + if
    + var
    + function
    + Object
    + Array

  + BOM

  + DOM

- Node.js 中的 JavaScript

  + 没有 BOM、DOM
  + EcmaScript 基本的 JavaScript 语言部分
  + 在 Node 中为 JavaScript 提供了一些服务器级别的 API
    * 文件操作的能力（例如文件的读写）
    * http 服务的能力
    * 网络服务的构建，网络通信

### Node.js能做什么

+ web服务器后台
+ 命令行工具
  + npm（node）
  + git(c语言)
  + hexo(node)
  + .....

+ 对于前端开发工程师来讲，接触node最多的是他的命令行工具
  + 自己写很少，主要是使用别人第三方的
  + webpack
  + gulp
  + npm

### 预备知识

+ HTML
+ CSS
+ JavaScript
+ 简单的命令行操作
  + cd
  + dir
  + ls
  + mkdir
  + rm

+ 具有服务端开发经验更佳

### node.js 学习资源

1. 图书

   - 《深入浅出Node.js》 作者：朴灵

   - 《node.js 实战 中国程序员6》

   - 《深入浅出Node.js》---底层原理----偏理论

     《Node.js权威指南》----API讲解

     JavaScript标准参考教程<http://javascript.ruanyifeng.com/>

     node入门 http://cnodejs.org

2. 网站资源

   - [CNODE社区](https://cnodejs.org/) 
   - [Node.js 简易教程](http://www.runoob.com/nodejs/nodejs-tutorial.html)
   - [Node入门](https://www.nodebeginner.org/index-zh-cn.html)
   - [Node.js包教不包会](https://github.com/ppker/node-lessons)
   - [CNODE-新手入门](http://cnodejs.org/getstart)
   - 其他参考链接
     - [Node.js 究竟是什么？](https://www.ibm.com/developerworks/cn/opensource/os-nodejs/index.html)
     - [Node.js是用来做什么的？](https://www.zhihu.com/question/33578075)
     - [什么是 node.js](http://www.infoq.com/cn/articles/what-is-nodejs)

3. Node.js 使用场景 & 实战

   - [Node.js雪球实战半年谈](http://www.undozen.com/slides/xueqiu2012a/#21.1)
   - [雪球上的 Node.js](http://mengxy.net/slides/nodejs-at-xueqiu/)
   - [国内有哪些网站使用了 Node.js](https://cnodejs.org/topic/50613e6601d0b8014822b6b9)
   - [Node.js & Uber](https://www.joyent.com/blog/node-js-office-hours-curtis-chambers-uber)
   - [Node.js 的优势和劣势](https://www.zhihu.com/question/19653241)
   - [node.js的15个应用场景](http://www.devstore.cn/essay/essayInfo/2199.html)
   - [How to decide when to use Node.js?](https://github.com/simongong/js-stackoverflow-highest-votes/blob/master/questions1-10/when-to-use-nodejs.md)
   - [优缺点及适用场景讨论](http://www.cnblogs.com/sysuys/p/3460614.html)
   - [Node.js 发展前景如何？适用于哪些场景？](https://www.zhihu.com/question/19587881)
   - [Node.js企业开发 一应用场景](http://n.thepana.com/2014/01/06/node-yingyong-changjing/)
   - [10个最佳Node.js企业应用案例：从Uber到LinkedIn](http://www.sohu.com/a/150175393_465223)
   - [极速Node.js：来自LinkedIn的10个性能提升秘籍](http://blog.jobbole.com/40135/)
   - 为分布式应用做中转
   - 前后端团队融合，节省成本
   - Node.js 简单高效
   - Node.js 是给前端用的，后端复杂的业务逻辑肯定不会用 Node.js

### 这门课能学到啥

+ B/S编程模型
  + Browser-Server
  + back-end
  + 任何服务端技术这种BS编程模型都是一样，和语言无关
  + Node只是作为我们学习BS编程模型的一个工具而已

+ 模块化编程
  + RequireJS
  + SeaJS
  + @import('文件路径')
  + 以前认知的JavaScript只能通过script标签来加载
  + 在node中可以向@import（)一样来引用加载JavaScript脚本文件
+ Node常用API
+ 异步编程
  + 回调函数
  + Promise
  + async
  + generator
+ Express开发框架
+ Ecmascript6
  + 新的语法
+ 。。。。。
+ 学习Node不仅会帮助大家打开服务端黑盒子，同时会帮助学习以后的前端高级内容
  + Vue.js
  + React
  + angular



## Node.js安装和配置

### node.js安装

1. 下载地址
   - [当前版本](https://nodejs.org/en/download/)
   - [历史版本](https://nodejs.org/en/download/releases/)
2. 官网术语解释
   - LTS 版本：Long-term Support 版本，长期支持版，即稳定版。
   - Current 版本：Latest Features 版本，最新版本，新特性会在该版本中最先加入。
3. 注意：
   - 安装完毕后通过命令：`node -v`来确定是否安装成功【注意：打开"命令窗口"的时候建议使用"管理员方式"打开】
   - 如果需要则配置环境变量。

![配置环境变量](C:/Users/ZOE%20XU/Desktop/node.js%E7%AC%94%E8%AE%B0/01-%E7%AC%94%E8%AE%B0%E5%A4%A7%E7%BA%B2/imgs/env_path.png)

通过 nvm-windows 管理一台计算机上的多个 node 版本

### node.js开发区别

**Node.js 开发 Web 应用程序 和 PHP、Java、ASP.Net等传统模式开发Web应用程序区别**

**传统模式**

- 有 Web 容器

![有Web容器开发模型](C:/Users/ZOE%20XU/Desktop/node.js%E7%AC%94%E8%AE%B0/01-%E7%AC%94%E8%AE%B0%E5%A4%A7%E7%BA%B2/imgs/Web.png)

**Node.js开发Web应用程序**

- 没有 Web 容器

![Node.js无Web容器开发模型](C:/Users/ZOE%20XU/Desktop/node.js%E7%AC%94%E8%AE%B0/01-%E7%AC%94%E8%AE%B0%E5%A4%A7%E7%BA%B2/imgs/nodeWeb.png)

### HelloWorld

1. 创建编写JavaScript脚本文件

2. 打开终端，定位到脚本文件所属目录

3. 输入node文件名，执行对应文件

注意:文件名不要使用 node.js 来命名，也就是说除了node随便起，而且最好也不要使用中文

+ 解析执行的JavaScript ---  

  ​	输入node 文件名，执行对应文件

  ​	在 Node 中，采用 EcmaScript 进行编码，没有 BOM、DOM                                                         

+ 读写文件----------

  + 读取文件

  ```js 
  // 浏览器中的 JavaScript 是没有文件操作的能力的
  // 但是 Node 中的 JavaScript 具有文件操作的能力
  
  // fs 是 file-system 的简写，就是文件系统的意思
  // 在 Node 中如果想要进行文件操作，就必须引入 fs 这个核心模块
  // 在 fs 这个核心模块中，就提供了所有的文件操作相关的 API
  // 例如：fs.readFile 就是用来读取文件的
  
  // 1. 使用 require 方法加载 fs 核心模块
  var fs = require('fs')
  
  // 2. 读取文件
  //    第一个参数就是要读取的文件路径
  //    第二个参数是一个回调函数
  //          
  //        成功
  //          data 数据
  //          error null
  //        失败
  //          data undefined没有数据
  //          error 错误对象
  fs.readFile('./data/hello.txt', function (error, data) {
    // <Buffer 68 65 6c 6c 6f 20 6e 6f 64 65 6a 73 0d 0a>
    // 文件中存储的其实都是二进制数据 0 1
    // 这里为什么看到的不是 0 和 1 呢？原因是二进制转为 16 进制了
    // 但是无论是二进制01还是16进制，人类都不认识
    // 所以我们可以通过 toString 方法把其转为我们能认识的字符
    // console.log(data)
  
    // console.log(error)
    // console.log(data)
  
    // 在这里就可以通过判断 error 来确认是否有错误发生
    if (error) {
      console.log('读取文件失败了')
    } else {
      console.log(data.toString())
    }
  });
  
  ```

  + 写文件

  ```javascript
  var fs = require('fs')
  
  // $.ajax({
  //   ...
  //   success: function (data) {
      
  //   }
  // })
  
  // 第一个参数：文件路径
  // 第二个参数：文件内容
  // 第三个参数：回调函数
  //    error
  //    
  //    成功：
  //      文件写入成功
  //      error 是 null
  //    失败：
  //      文件写入失败
  //      error 就是错误对象
  fs.writeFile('./data/你好.md', '大家好，给大家介绍一下，我是Node.js', function (error) {
    // console.log('文件写入成功')
    // console.log(error)
    if (error) {
      console.log('写入失败')
    } else {
      console.log('写入成功了')
    }
  })
  ```

+ http

  + 创建服务器

```js
// 接下来，我们要干一件使用 Node 很有成就感的一件事儿
// 你可以使用 Node 非常轻松的构建一个 Web 服务器
// 在 Node 中专门提供了一个核心模块：http
// http 这个模块的职责就是帮你创建编写服务器的

// 1. 加载 http 核心模块
var http = require('http')

// 2. 使用 http.createServer() 方法创建一个 Web 服务器
//    返回一个 Server 实例
var server = http.createServer()

// 3. 服务器要干嘛？
//    提供服务：对 数据的服务
//    发请求
//    接收请求
//    处理请求
//    给个反馈（发送响应）
//    注册 request 请求事件
//    当客户端请求过来，就会自动触发服务器的 request 请求事件，然后执行第二个参数：回调处理函数
server.on('request', function () {
  console.log('收到客户端的请求了')
})

// 4. 绑定端口号，启动服务器
server.listen(3000, function () {
  console.log('服务器启动成功了，可以通过 http://127.0.0.1:3000/ 来进行访问')
})
```

http-res

```js 
var http = require('http')

var server = http.createServer()

// request 请求事件处理函数，需要接收两个参数：
//    Request 请求对象
//        请求对象可以用来获取客户端的一些请求信息，例如请求路径
//    Response 响应对象
//        响应对象可以用来给客户端发送响应消息
server.on('request', function (request, response) {
  // http://127.0.0.1:3000/ /
  // http://127.0.0.1:3000/a /a
  // http://127.0.0.1:3000/foo/b /foo/b
  console.log('收到客户端的请求了，请求路径是：' + request.url)

  // response 对象有一个方法：write 可以用来给客户端发送响应数据
  // write 可以使用多次，但是最后一定要使用 end 来结束响应，否则客户端会一直等待
  response.write('hello');
  response.write(' nodejs');

  // 告诉客户端，我的话说完了，你可以呈递给用户了
  response.end();

  // 由于现在我们的服务器的能力还非常的弱，无论是什么请求，都只能响应 hello nodejs
  // 思考：
  //  我希望当请求不同的路径的时候响应不同的结果
  //  例如：
  //  / index
  //  /login 登陆
  //  /register 注册
  //  /haha 哈哈哈
})

server.listen(3000, function () {
  console.log('服务器启动成功了，可以通过 http://127.0.0.1:3000/ 来进行访问')
})
```

### Node 中的 JavaScript

+ ECMAScript
  + 没有DOM BOM

+ 核心模块

+ 第三方模块

+ 用户自定义模块

  #### 核心模块

  Node为JavaScript提供了很多服务器级别的API，这些API绝大多数都被包装到了一个具名的核心模块中了。

  例如文件操作的 fs 核心模块，http服务构建的 http 模块， path 路径操作模块 ， os 操作系统模块。。

  必须引入

  ```js
  var fs =require('fs')
  var http=require('http')
  ```

  #### 用户自定义模块

  - require

  - exports

    ```js
    // require 是一个方法
    // 它的作用就是用来加载模块的
    // 在 Node 中，模块有三种：
    //    具名的核心模块，例如 fs、http
    //    用户自己编写的文件模块
    //      相对路径必须加 ./
    //      可以省略后缀名
    //      相对路径中的 ./ 不能省略，否则报错
    //    在 Node 中，没有全局作用域，只有模块作用域
    //      外部访问不到内部
    //      内部也访问不到外部
    //      默认都是封闭的
    //    既然是模块作用域，那如何让模块与模块之间进行通信
    //    有时候，我们加载文件模块的目的不是为了简简单单的执行里面的代码，更重要是为了使用里面的某个成员
    
    var foo = 'aaa'
    
    console.log('a start')
    
    function add(x, y) {
      return x + y
    }
    
    // Error: Cannot find module 'b'
    // require('b')
    
    // 可以
    // require('./b.js')
    
    // 推荐：可以省略后缀名
    require('./b')
    
    console.log('a end')
    
    console.log('foo 的值是：', foo)
    ```

```js
// require 方法有两个作用：
//    1. 加载文件模块并执行里面的代码
//    2. 拿到被加载文件模块导出的接口对象
//    
//    在每个文件模块中都提供了一个对象：exports
//    exports 默认是一个空对象
//    你要做的就是把所有需要被外部访问的成员挂载到这个 exports 对象中
var bExports = require('./b')
var fs = require('fs')

console.log(bExports.foo)

console.log(bExports.add(10, 30))

console.log(bExports.age)

bExports.readFile('./a.js')

fs.readFile('./a.js', function (err, data) {
  if (err) {
    console.log('读取文件失败')
  } else {
    console.log(data.toString())
  }
})
```

![](.\images\ip地址和端口号.png)



## 总结

- Node 中的 JavaScript
  + EcmaScript
    * 变量
    * 方法
    * 数据类型
    * 内置对象
    * Array
    * Object
    * Date
    * Math
  + 模块系统
    * 在 Node 中没有全局作用域的概念
    * 在 Node 中，只能通过 require 方法来加载执行多个 JavaScript 脚本文件
    * require 加载只能是执行其中的代码，文件与文件之间由于是模块作用域，所以不会有污染的问题
      - 模块完全是封闭的
      - 外部无法访问内部
      - 内部也无法访问外部
    * 模块作用域固然带来了一些好处，可以加载执行多个文件，可以完全避免变量命名冲突污染的问题
    * 但是某些情况下，模块与模块是需要进行通信的
    * 在每个模块中，都提供了一个对象：`exports`
    * 该对象默认是一个空对象
    * 你要做的就是把需要被外部访问使用的成员手动的挂载到 `exports` 接口对象中
    * 然后谁来 `require` 这个模块，谁就可以得到模块内部的 `exports` 接口对象
    * 还有其它的一些规则，具体后面讲，以及如何在项目中去使用这种编程方式，会通过后面的案例来处理
  + 核心模块
    * 核心模块是由 Node 提供的一个个的具名的模块，它们都有自己特殊的名称标识，例如
      - fs 文件操作模块
      - http 网络服务构建模块
      - os 操作系统信息模块
      - path 路径处理模块
      - 。。。。
    * 所有核心模块在使用的时候都必须手动的先使用 `require` 方法来加载，然后才可以使用，例如：
      - `var fs = require('fs')`
- http
  + require
  + 端口号
    * ip 地址定位计算机
    * 端口号定位具体的应用程序
  + Content-Type
    * 服务器最好把每次响应的数据是什么内容类型都告诉客户端，而且要正确的告诉
    * 不同的资源对应的 Content-Type 是不一样，具体参照：http://tool.oschina.net/commons
    * 对于文本类型的数据，最好都加上编码，目的是为了防止中文解析乱码问题
  + 通过网络发送文件
    * 发送的并不是文件，本质上来讲发送是文件的内容
    * 当浏览器收到服务器响应内容之后，就会根据你的 Content-Type 进行对应的解析处理

- 模块系统
- Node 中的其它的核心模块
- 做一个小管理系统：
  + CRUD
- Express Web 开发框架
  + `npm install express`
