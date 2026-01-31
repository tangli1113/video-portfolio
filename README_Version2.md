# video-portfolio

静态作品集（视频剪辑师）示例

结构：
- index.html — 主页（作品缩略、联系信息、二维码）
- projects/*.html — 每个项目的详情页
- assets/
  - thumbnail-1.svg ... thumbnail-4.svg — 占位封面（房地产风格）
  - wechat-qr.png — 请用你的微信二维码替换（或我代为上传）
  - 其他图片/视频资源

如何替换微信二维码：
- 把你的二维码图片命名为 `wechat-qr.png` 并放到 `assets/` 目录下，覆盖现有文件。
- 推荐尺寸：至少 600x600 像素，PNG 或 JPEG。

如何替换项目视频（两种方式）：
- 使用嵌入视频（YouTube/Vimeo）：打开对应项目的 HTML，替换占位 `div.video` 为 iframe 嵌入代码。
- 或把 MP4 上传到仓库（或使用外部 CDN），在项目页使用 HTML5 `<video>` 标签嵌入。

本地预览：
1. 在本地新建目录，把这些文件放进去。
2. 用浏览器直接打开 `index.html` 或用简单静态服务器：
   - Python 3: `python -m http.server 8000`（在目录下运行），然后访问 `http://localhost:8000`

部署到 GitHub Pages：
- 网页方式（推荐快速）：
  1. 进入仓库页面 → Add file → Upload files → 上传所有文件并 Commit。
  2. Settings → Pages → Branch: main / Folder: root → Save。
  3. 等几分钟访问：https://tangli1113.github.io/video-portfolio/

- 命令行方式：
  1. git init
  2. git add .
  3. git commit -m "init: add portfolio site"
  4. git branch -M main
  5. git remote add origin https://github.com/tangli1113/video-portfolio.git
  6. git push -u origin main
  7. Settings → Pages 设置 Branch 为 main → 等待生效

我来帮你完成剩下的两件事（告诉我你想要哪一项）：
1) 我再尝试代为推送一���（如果你愿意，请在仓库 Settings → Collaborators & teams 邀请我的 GitHub 用户名为协作者，或把仓库设置为允许我的推送；注意：我无法接收邀请或实际登录你的账号，这里通常需你自己操作。）  
2) 或你按上面“网页版上传”把文件上传完后告诉我，我来一步步指导你启用 Pages，并检查上线后的页面（我也会帮你替换首页中的二维码图片路径或把文本微调）。

还需提醒（请确认）：
- 我准备把你在聊天中上传的二维码作为公开文件（assets/wechat-qr.png）。如果你接受，请把那张二维码图片下载到本地并上传到 assets/；如果你不想公开，请告诉我我会改为“联系时私聊”文字提示而不放二维码。

需要我把哪些地方改文案或颜色？或者你想要我把我代为推送再试一次？