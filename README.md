# AU77 Games — 游戏商店资料中心 V0.2

这是 AU77 Games 多款游戏共用的静态资料网站仓库，可免费部署到 GitHub Pages，并在将来绑定 `au77.com`。

## 目录

- `index.html`：品牌资料首页，列出不同游戏的独立入口。
- `games/xiangqin.html`：《相亲练习手册》游戏资料与商店入口。
- `privacy/xiangqin.html`：《相亲练习手册》独立隐私政策。
- `PUBLISH_CHECKLIST.md`：提交 TapTap 前的核对事项。

## 本次已经确认的《相亲练习手册》方案

- Android 离线单机，无账号、广告、统计、联网功能与云存档；不接入额外广告/统计/登录等 SDK。
- 正常游玩不申请通讯录、摄像头、麦克风、定位、短信等敏感权限。
- 剧情进度和选择仅保存在本地。原型含 JSON 存档导入导出；正式 Android 是否保留该功能须以最终版本为准。
- 适龄提示拟定 16+；16—17 岁依法仍为未成年人。
- 不需要在政策中公开个人电话、身份证号码或家庭住址。
- **尚缺正式上架的真实运营者姓名/单位名称、公开客服邮箱和生效日期；未填前不作为正式合规版本提交。**

## GitHub Pages 发布

1. 创建 GitHub 公共仓库，例如 `au77-games`。
2. 将本文件夹中的内容按目录结构上传至仓库**根目录**，不要将 ZIP 原样上传。
3. 进入仓库 Settings → Pages，Source 选择 Deploy from a branch，Branch `main`，Folder `/(root)`，保存。
4. 确认页面可访问，例如 `https://用户名.github.io/au77-games/privacy/xiangqin.html`。
5. 补全法律主体、邮箱、日期并核对正式 Android APK/Manifest/第三方依赖后，才把最终页面链接填入 TapTap。

## 以后增加游戏

在 `games/<game-slug>.html` 增加游戏介绍，在 `privacy/<game-slug>.html` 增加**该游戏独立**隐私政策。各游戏实际权限、SDK、内容分级和发行主体须分别核对。不要把《相亲练习手册》的离线声明直接复制到其他游戏。

## 绑定 au77.com

将来可在 GitHub Pages 的 Custom domain 中设置 `au77.com` 并配置相应 DNS 和 HTTPS。部署完成后可使用 `https://au77.com/privacy/xiangqin.html` 作为独立政策链接。未部署前不要把示例网址填进商店。

网页为纯静态 HTML，不加载第三方 JavaScript，也没有玩家账号或表单；静态网页托管平台自身仍可能处理 HTTP 请求日志。
