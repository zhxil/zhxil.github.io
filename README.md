# zhxil GitHub Pages — 个人网站 V0.2

四项精选作品：**CodexWatch / iPhoneStock / LumaConvert / ContentFactory**。静态 HTML、CSS、JavaScript，无需构建工具、账号登录或后端。

## 预览

直接打开 `index.html` 即可，也可运行 `python -m http.server 8000` 并访问 `http://localhost:8000`。

## 发布到 GitHub Pages

1. 在 GitHub 账号 `zhxil` 中创建名为 `zhxil.github.io` 的 **Public** 仓库。
2. 将本 `site/` 目录内所有文件上传到仓库根目录（不要再套一层 `site/`）。
3. 进入 Settings → Pages → Build and deployment，选择 Deploy from a branch，选 `main` 和 `/(root)`，保存。
4. 待 GitHub 部署完成后，访问 `https://zhxil.github.io`。

## 更新

- 网站样式：`assets/style.css`
- 内容：`index.html` 和 `projects/*.html`
- GitHub 原始截图：项目对应仓库的 `docs/screenshots` 或 `docs/images` 路径；当前是远程加载，可以按需改为本地素材。
- 点击导航对应 `#work`、`#about`、`#notes` 和 `#contact`。
- `#notes` 目前只是预留介绍区，没有虚构文章。

## 注意

项目描述来源于仓库公开 README，发布前应复核个人简介和技术栈是否需要调整。iPhoneStock 的上游协议参考与 GPL 许可说明必须保留。网站仅是项目展示，不在 GitHub Pages 运行 Python 或原生客户端。

## V0.2 更新

- 新增 LumaConvert（轻转）项目卡片及完整详情页，使用 GitHub 仓库中的真实截图。
- 精选项目改为两列 × 两行布局。
- 仍不包含 Fork 项目，且不会把外部仓库作为原创项目。
