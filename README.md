# Node.js Koa2框架搭建电影预告片网站
- Node.js Koa2 the movie trailer site

- 视频课程出品时间：2018年

----

## 课程大纲
- [第1章 2018 年的编程姿势](#第1章-2018-年的编程姿势)
    - [1-1 koa2导学](#1-1-koa2导学)
    - [1-2 安装跟进最新 node.js 版本](#1-2-安装跟进最新-node.js-版本)
    - [1-3 毫不犹豫的使用promise](#1-3-毫不犹豫的使用promise)
    - [1-4 使用babel 编译es7 async function](#1-4-使用babel-编译es7-async-function)
- [第2章 必会 ES6-7 语法特性与规范](#第2章-必会-ES6-7-语法特性与规范)
    - [2-1 生成器函数 Iterator迭代器？](#2-1-生成器函数-Iterator迭代器？)
    - [2-2 co 库执行 promise 和 generator function](#2-2-co-库执行-promise-和-generator-function)
    - [2-3 箭头函数 arrow function](#2-3-箭头函数-arrow-function)
    - [2-4 异步函数 asyunc function 统一世界](#2-4-异步函数-asyunc-function-统一世界)
    - [2-5 借助 babel 编译 import 与 export](#2-5-借助-babel-编译-import-与-export)
    - [2-6 生产环境使用 babel 支持 es6-7](#2-6-生产环境使用-babel-支持-es6-7)
- [第3章 层层学习 Koa 框架的 API](#第3章-层层学习-Koa-框架的-API)
    - [3-1 koa 核心对象](#3-1-koa-核心对象)
    - [3-2 web服务类 application](#3-2-web服务类-application)
    - [3-3 http 上下文对象 context（ctx）](#3-3-http-上下文对象-context（ctx）)
    - [3-4 http 请求对象 request（req）](#3-4-http-请求对象-request（req）)
    - [3-5 http 响应对象](#3-5-http-响应对象)
    - [3-6 koa 中间件 middlewares](#3-6-koa-中间件-middlewares)
    - [3-7 纯函数-尾递归与魔法大师 koa-compose](#3-7-纯函数-尾递归与魔法大师-koa-compose)
    - [3-8 session-cookie-路由 koa小结](#3-8-session-cookie-路由-koa小结)
- [第4章 Koa2 与 Koa1 、Express 框架对比](#第4章-Koa2-与-Koa1-、Express-框架对比)
    - [4-1 koa2与koa1 的用法对比](#4-1-koa2与koa1-的用法对比)
    - [4-2 koa 与 express 的api 能力对比](#4-2-koa-与-express-的api-能力对比)
    - [4-3 koa 与 express的中间件执行模板对比](#4-3-koa-与-express的中间件执行模板对比)
    - [4-4 koa2 espress 选型及小结（含奖励哦）](#4-4-koa2-espress-选型及小结（含奖励哦）)
- [第5章 从 0 开发一个电影预告片网站](#第5章-从-0-开发一个电影预告片网站)
    - [5-1 设计与分析](#5-1-设计与分析)
    - [5-2 行代码撸一个服务器推到git仓库](#5-2-行代码撸一个服务器推到git仓库)
    - [5-3 服务器返回一个静态 html页面](#5-3-服务器返回一个静态-html页面)
    - [5-4 集成模板引擎 koa 搭建初始模板目录](#5-4-集成模板引擎-koa-搭建初始模板目录)
    - [5-5 集成模板引擎到koa 搭建初始模板目录](#5-5-集成模板引擎到koa-搭建初始模板目录)
    - [5-6 借助 bootstrap 4-x 搭建网站首页](#5-6-借助-bootstrap-4-x-搭建网站首页)
- [第6章 利用爬虫搞定网站基础数据](#第6章-利用爬虫搞定网站基础数据)
    - [6-1 设计与分析](#6-1-设计与分析)
    - [6-2 利用 puppeteer 爬取和分析电影列表](#6-2-利用-puppeteer-爬取和分析电影列表)
    - [6-3 child_process fork 子进程来运行爬虫脚本](#6-3-child_process-fork-子进程来运行爬虫脚本)
    - [6-4 服务器端通过 request 向豆瓣 api 请求详细数据](#6-4-服务器端通过-request-向豆瓣-api-请求详细数据)
    - [6-5 scott 与妹子合租引发的同步异步与阻塞](#6-5-scott-与妹子合租引发的同步异步与阻塞)
    - [6-6 puppeteer 深度爬取封面图和视频地址](#6-6-puppeteer-深度爬取封面图和视频地址)
    - [6-7 上传线上封面图和视频搬砖到七牛云图床上](#6-7-上传线上封面图和视频搬砖到七牛云图床上)
- [第7章 彩蛋篇 - [高难度拔高干货] 深度理解 Node.js 异步 IO 模型](#第7章-彩蛋篇---[高难度拔高干货]-深度理解-Node.js-异步-IO-模型)
    - [7-1 从异步非阻塞的代码案例切入事件循环](#7-1-从异步非阻塞的代码案例切入事件循环)
    - [7-2 从异步非阻塞的代码案例切入事件循环](#7-2-从异步非阻塞的代码案例切入事件循环)
    - [7-3 从libuv 源码来理解event loop的六个阶段](#7-3-从libuv-源码来理解event-loop的六个阶段)
    - [7-4 设计一个测试用例来验证自己对事件循环的理解](#7-4-设计一个测试用例来验证自己对事件循环的理解)
- [第8章 实战篇 - 在 Koa 中向 MongoDB 建立数据模型](#第8章-实战篇---在-Koa-中向-MongoDB-建立数据模型)
    - [8-1 windows mac centos ubuntu安装mongodb-1](#8-1-windows-mac-centos-ubuntu安装mongodb-1)
    - [8-2 koa2 中利用 mongoose链接数据库](#8-2-koa2-中利用-mongoose链接数据库)
    - [8-3 mongodb和mongoose关于 collection schema model entity 的基本](#8-3-mongodb和mongoose关于-collection-schema-model-entity-的基本)
    - [8-4 利用 schema model创建电影的数据模型](#8-4-利用-schema-model创建电影的数据模型)
    - [8-5 创建用户数据模型并实现加盐加密和敏感登控制](#8-5-创建用户数据模型并实现加盐加密和敏感登控制)
    - [8-6 创建电影分类以及初始化所有](#8-6-创建电影分类以及初始化所有)
    - [8-7 向数据库导入爬到的电影数据](#8-7-向数据库导入爬到的电影数据)
- [第9章 实战篇 - 为网站增加路由与控制器层对外提供 API 服务](#第9章-实战篇---为网站增加路由与控制器层对外提供-API-服务)
    - [9-1 第二次迭代快速实现一个最小统计的api服务器](#9-1-第二次迭代快速实现一个最小统计的api服务器)
    - [9-2 第二次迭代了解koa-router的基本能力以及取舍套路](#9-2-第二次迭代了解koa-router的基本能力以及取舍套路)
    - [9-3 通过装饰器来把路由进行拆分和继承](#9-3-通过装饰器来把路由进行拆分和继承)
    - [9-4 结合decorator 对 koa-router 进行抽象封装支持路由空间](#9-4-结合decorator-对-koa-router-进行抽象封装支持路由空间)
    - [9-5 分拆项目服务层与路由层对外暴露api服务](#9-5-分拆项目服务层与路由层对外暴露api服务)
- [第10章 实战篇 - 集成 AntDesign 与 Parcel 打通前后端与构建](#第10章-实战篇---集成-AntDesign-与-Parcel-打通前后端与构建)
    - [10-1 第三次迭代 配置babel postcss来支持 parcel 的打包构建](#10-1-第三次迭代-配置babel-postcss来支持-parcel-的打包构建)
    - [10-2](#10-2)
    - [10-3 第三次迭代 结合 react-router-dom 与import 来动态加载前端路由](#10-3-第三次迭代-结合-react-router-dom-与import-来动态加载前端路由)
    - [10-4 第三次迭代 实现网站的布局模板组件和导航菜单](#10-4-第三次迭代-实现网站的布局模板组件和导航菜单)
- [第11章 实战篇 - 实现网站前端路由与页面功能](#第11章-实战篇---实现网站前端路由与页面功能)
    - [11-1 第四次迭代 axios封装可控制](#11-1-第四次迭代-axios封装可控制)
    - [11-2 第四次迭代 开发网站首页电影列表](#11-2-第四次迭代-开发网站首页电影列表)
    - [11-3 第四次迭代 抽象网站首页电影卡片内容组件](#11-3-第四次迭代-抽象网站首页电影卡片内容组件)
    - [11-4 第四次迭代 为电影卡片增加视频播放及切换功能](#11-4-第四次迭代-为电影卡片增加视频播放及切换功能)
    - [11-5 第四次迭代 开发电影详情页](#11-5-第四次迭代-开发电影详情页)
- [第12章 实战篇 - 实现后台登录权限与管理功能](#第12章-实战篇---实现后台登录权限与管理功能)
    - [12-1 实现网站的后端登录页面及密码校检](#12-1-实现网站的后端登录页面及密码校检)
    - [12-2 实现网站后端管理列表页](#12-2-实现网站后端管理列表页)
    - [12-3 增加登录权限](#12-3-增加登录权限)
    - [12-4 增加用户会话](#12-4-增加用户会话)
- [第13章 服务器部署与发布](#第13章-服务器部署与发布)
    - [13-1 简单配置本地与服务器](#13-1-简单配置本地与服务器)
    - [13-2 服务器第一次部署与发布](#13-2-服务器第一次部署与发布)
- [第14章 课程总结与展望](#第14章-课程总结与展望)
    - [14-1 koa2 课程回顾总结](#14-1-koa2-课程回顾总结)

----


# 第1章 2018 年的编程姿势
- ## 1-1 koa2导学
    - 市场常见 Node.js Web 服务框架
        - Express
        - Koa
        - Sail
        - Hapi
    - 本课程概况
        - 做什么？
            - 开发一个可以实时更新的预告片网站
        - 有哪些功能？
            - 网站首页
            - 网站首页播放窗口
            - 网站播放详情页
            - 网站详情
            - 同类推荐
            - 网站后台登陆
            - 网站后台管理列表
        - 技术栈？
            - Koa2
            - Nodejs
            - MongoDB
            - Puppeteer
            - Parcel
            - AntDesign
    - 解答 过去我们 遇到的问题？
        - Koa 框架到底为我们做了什么？
        - 他的内部到底是什么样子？
        - 他向下一直到 Node.js 底层，到底是怎么处理事件循环的？
        - 一个异步的 HTTP 过程，到底是怎么样进行的？

- ## 1-2 安装跟进最新 node.js 版本
    - https://node.green/
        - 查看 当前阶段 各个Node.js版本 对ECMA规范 实现的程度，及支持情况
    - NVM
        - 问题：本地如何管理 那么多的 Node.js 版本？
        - 什么是 NVM？
            - Node.js版本管理工具
        - 使用 NVM 这个 Node.js版本管理工具
        - 如何安装 NVM ？
            - 到 github [搜索](https://github.com/search?o=desc&q=nvm&s=stars&type=Repositories)
            - Mac / Linux 安装 NVM 方式
                - ```curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash```
            - 由于 Windows 和 Mac / Linux 的安装方式不同
                - [《nvm-windows github》Windows 安装 NVM](https://github.com/coreybutler/nvm-windows)
                - [nvm介绍 安装 及使用](https://www.jianshu.com/p/d0e0935b150a)
    - 如何使用 NVM
        ```shell
        nvm ls              #查看本地安装的node版本
        nvm install stable  # 安装最新稳定版 node，现在是 5.0.0
        nvm install 4.2.2   # 安装 4.2.2 版本
        nvm install 0.12.7  # 安装 0.12.7 版本

        # 特别说明：以下模块安装仅供演示说明，并非必须安装模块
        nvm use 4           # 切换至 4.2.2 版本
        npm install -g mz-fis # 安装 mz-fis 模块至全局目录，安装完成的路径是 /Users/<你的用户名>/.nvm/versions/node/v0.12.7/lib/mz-fis
        nvm use 0           # 切换至 0.12.7 版本
        npm install -g react-native-cli #安装 react-native-cli 模块至全局目录，安装完成的路径是 /Users/<你的用户名>/.nvm/versions/node/v4.2.2/lib/react-native-cli

        nvm alias default 0.12.7 #设置默认 node 版本为 0.12.7
        ```


- ## 1-3 毫不犹豫的使用promise
    - Promises 官网
        - https://www.promisejs.org/
    - Promises 是什么？
        - Promises 不是一个简单的语法糖
        - 而是一个规范
            - 如 bluebird 就实现了这个规范
        - 各种各样的库 都可以去实现这套规范，进而向我们 提供Promises能力的接口 函数
    - ### 1.在过去 我们使用 **回调方式**
        ```js
        const fs = require('fs')

        // 1.回调方式
        fs.readFile('./1-3 Promise.js', (err, data) =>{
            if (err) throw err

            console.log(data.toString())
        })
        ```
    - ### 2.使用Promise 过渡时期 (2017左右)
        ```js
        const fs = require('fs')

        function readFileAsync (path) {
            return new Promise((resolve, reject) => {
                fs.readFile(path, (err, data) => {
                    if (err) reject(err)
                    else resolve(data)
                })
            })
        }

        readFileAsync('./1-3 Promise.js')
            .then(data => {
                console.log(data.toString())
            })
            .catch(err => {
                console.log(err)
            })
        ```
        - 虽然这种写法 有点冗长，但是也没有什么弊端
    - ### 3.现在 util 的 promisify
        - Node.js 进入 v8.x 版本以后
        - 我们就可以使用 nodejs util 模块提供的 promisify 让我们可以轻易的 包装一个 回调式的 Api ，让它直接支持 promise
        ```js
        const fs = require('fs')
        const util = require('util')

        util.promisify(fs.readFile)('./1-3 Promise.js')
            .then(data => {
                console.log(data.toString())
            })
            .catch(err => {
                console.log(err)
            })
        ```
        - 解释
            - ```util.promisify()```
                - 传入某一个回调函数，这里传入 fs.readFile ，fs.readFile 它本身是一个回调的异步函数
            - ```util.promisify(fs.readFile)```
                - 我们把这个函数包装之后，它会返回一个 promise function，再来调用
            - ```util.promisify(fs.readFile)('./1-3 Promise.js')```
                - 后面的这个 () 才是传参数
        - 总结
            - 优点：减少了代码量。将原来 promise 方法中的 20行代码，减少到 10行
            - 在项目中遇到有 **回调处理异步的场景**，推荐大家 使用这种 promisify，来完成 从回调到 向promise 迁移到工作


- ## 1-4 使用babel 编译es7 async function
    - 先来看 这段 使用 async function 实现 上一节中的同样的功能
    ```js
    const fs = require('fs')
    const util = require('util')
    const readAsync = util.promisify(fs.readFile)

    async function init () {
        try {
            let data = await readAsync('./1-3 Promise.js')
            console.log(data.toString())
        } catch (err) {
            console.log(err)
        }
    }

    init()
    ```
    - 存在的问题
        - 使用这些新的语法，虽然用起来很爽
        - 但是，也带来一些问题
            - 当你的运行环境不支持 这些前卫的新语法时，就会导致无法正确运行代码。
            - 如：你在node v4.x 或者 v6.x 版本中使用时
        - 所以这个时候，就需要用到 babel 来编译，将这些 旧版本不支持的新语法，编译成 他们能够识别执行的语法

# 第2章 必会 ES6-7 语法特性与规范
- ## 2-1 生成器函数 Iterator迭代器？
    - generator function
        - generator function 是 ES6 新增的特性，node.js v4.x 版本后就可以直接使用了
        - generator function 的核心是 ```generator 生成器```
        - ```generator 生成器``` 的本质是 ```Iterator 迭代器```
        - 所以我们先要理解，什么是 ```Iterator 迭代器``` 这个概念
    - ### 什么是 Iterator 迭代器？
        - Iterator 迭代器
            - 跟 Promise 一样，并不是 某一个具体的语法 或者 对象
            - 它是一个 **协议**
            - 只要遵循这个 协议 所实现的，都是迭代器对象
        - 下面来手写一个 Iterator 迭代器
            ```js
            function makeIterator (arr) {
                let nextIndex = 0

                // 返回一个迭代器对象
                return {
                    next: () => {
                        // next() 方法返回的结果对象
                        if (nextIndex < arr.length) {
                            return { value: arr[nextIndex++], done: false }
                        } else {
                            return { done: true }
                        }
                    }
                }
            }

            const it = makeIterator(['吃饭', '睡觉', '打豆豆'])

            console.log('首先', it.next().value)
            console.log('其次', it.next().value)
            console.log('然后', it.next().value)
            console.log('最后', it.next().done)

            // 打印结果
            首先 吃饭
            其次 睡觉
            然后 打豆豆
            最后 true
            ```
            - 这是一个非常简易的 Iterator 迭代器
            
    - ### Iterator 迭代器 特征
            - 每一次迭代的值，都是跟上一次迭代的值 有关系的，它是处于上一个值，下一个序列中 即将被执行的链路
            - 每一次迭代的值，都反映了 迭代器内部的状态
            - 这些状态的组合 是一个完整的状态流程
            - 我们通过 next 方法，依次拿到某个状态的值
            - 迭代器内部 总有一个 next 方法，通过它 总能拿到一个对象
            - 其中 value 是某一次迭代的结果，done 是当前是否迭代完成的标志



- ## 2-2 co 库执行 promise 和 generator function
- ## 2-3 箭头函数 arrow function
- ## 2-4 异步函数 asyunc function 统一世界
- ## 2-5 借助 babel 编译 import 与 export
- ## 2-6 生产环境使用 babel 支持 es6-7