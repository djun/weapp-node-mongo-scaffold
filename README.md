# weapp-koa2-mongo-scaffold
此项目为微信小程序与mongodb数据交互解决方案，使用koa + mongodb结构，jwt鉴权

## 开始使用

1. Clone项目
```
git clone https://github.com/seawind8888/weapp-koa2-mongo-scaffold my-project
```

2. 安装依赖
```
cd my-porject
npm install 或 yarn
```


3. 参数设置
```
confing/index.js设置参数

app: {
    port: 3008, // 项目开启端口
    whiteList: [/\/user\/login/]  // 无需session验证白名单
},
weapp: {
    AppID: "xxx", // 微信AppID
    AppSecret: "xxxxxx" 微信AppSecret
}
```

4. 运行项目

```
npm run dev
```

## 目录结构
```
├── config/ 
│ ├── index.js            # 项目参数设置
├── controllers/          # 处理路由映射函数中心
├── controllers/          # 小程序示例项目
├── middleware/           # 中间件目录
├── model/                # mongo模型目录
├── routes/               # koa路由目录
├── .babelrc              # babel配置
├── app.js                # 项目启动模块
├── index.js              # 项目启动入口
├── pm2.config.json       # pm2配置目录
└──  package.json         # 项目信息
```