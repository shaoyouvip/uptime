# uptime

一个基于 UptimeRobot API 的在线状态面板

<img width="1152" alt="image" src="https://user-images.githubusercontent.com/25887822/178935137-6d23521d-5894-4fb8-922d-3575be4f7abc.png">

## 事先准备

- 您需要先到 [UptimeRobot](https://uptimerobot.com/ "UptimeRobot") 添加站点监控，并在`integrations&API`中`Main API keys`获取`Read-only API key`格式为`ur2671488-fb491a80091166a48bc66b17`这是我的只读API，你需要 修改 `config.js` 文件`ApiKeys`中替换为你的。
- 您需要拥有一个网站空间，常见的 Nginx / PHP 等空间即可，甚至是阿里云的 OSS 等纯静态空间也行

## 如何部署：

- 下载并解压缩本项目的文件：[uptime.zip]
- 修改 `config.js` 文件：
   - `SiteName`: 要显示的网站名称
   - `ApiKeys`: 从 UptimeRobot 获取的 API Key，支持 Monitor-Specific API Keys 和 Read-Only API Key
   - `CountDays`: 要显示的日志天数，建议 60 或 90，显示效果比较好
   - `ShowLink`: 是否显示站点链接
   - `Navi`: 导航栏的菜单列表
- 将所有文件上传到网站空间

⚠️ 如果没有修改代码的需求，您不需要 git clone 本项目，只需要下载 Release 的文件包即可。

## 鸣谢：

 [uptime-status](https://github.com/yb/uptime-status/ "uptime-status")
