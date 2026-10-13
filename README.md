# NURS513 互动复习

此仓库包含静态入口、加密学习内容、图标与离线缓存。无需安装依赖、数据库或服务端。

## 发布到 GitHub Pages

1. 把本包内的所有文件放到公开仓库根目录，确保 index.html 直接在根目录。
2. 仓库 Settings → Pages → Build and deployment，Source 选择 Deploy from a branch。
3. Branch 选择 main（或实际默认分支），Folder 选择 / (root)，点击 Save。
4. 发布成功后，在 Pages 设置中打开显示的网站地址。项目站通常为 https://用户名.github.io/仓库名/。

参考：[GitHub 官方发布说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## 内容保护

课程内容以 AES-256-GCM 加密，密钥由用户输入经 PBKDF2-SHA256（600,000 次）导出。密码与明文讲义不在此包中；不要把原始课件、未加密学习册或个人进度备份加入公开仓库。进入密码由持有人另行提供。简单密码仍可被猜到；此方式用于轻度访问限制，并非服务端身份验证。

“在此设备保持解锁”将解密密钥保存在该浏览器本机；“锁定”清除此密钥。进度和错题独立保留。不能把保持解锁的设备当作受密码保护的设备。

## 使用

- 手机和电脑都能打开；可在 Safari 分享菜单中添加到主屏幕。
- 随机选择题即时核对；英文短答和概念卡需对照示例自行评价。
- 可按周筛选，练错题，或隐藏中文。
- 进度保存在本机，可导出 JSON 并在另一台设备导入。不会自动云同步。
- HTTPS 发布后首次在线打开会尝试缓存加密网页，以便断网时继续；能否离线使用取决于浏览器缓存，未完成线上部署前无法实机验证。

本包仅上传加密页面；用户应自行管理课程资料的分享权限。
