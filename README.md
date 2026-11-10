# 造梦工作台

造梦先生的个人工作台：今日计划、在谈客户、方案进度、工地动态、问题追踪、抖音排期、每周复盘。

- 这是一个纯静态网页应用（`index.html` 单文件 + PWA 清单 + 图标）。
- **仓库里只有程序空壳，没有任何个人数据。** 所有记录只存在使用者自己的设备里；双端同步走 `edge-functions/api/sync.js`（EdgeOne Pages 边缘函数 + Blob 存储），同步密码在页面内设置、服务端哈希存储，不经过本仓库。
- 部署方式：EdgeOne Pages 从本仓库 Git 导入（同步函数依赖 `@edgeone/pages-blob`，需平台自动执行 `npm install`，见 `package.json`）。
- 由「不一书个人工作台生成器」(bys-personal-dashboard) 生成。
