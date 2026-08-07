# 辛炬 · 个人简历网站

这是一个无需构建工具的静态网站，可直接部署到 GitHub Pages。

## 文件结构

```text
xinju-resume-site/
├── index.html
├── styles.css
├── script.js
└── assets/
    ├── favicon.svg
    └── headshot.jpg
```

## 本地预览

在当前目录运行：

```bash
python3 -m http.server 8000
```

然后访问 `http://localhost:8000`。

## 发布到 GitHub Pages

1. 在 GitHub 创建公开仓库，例如 `resume`。
2. 将本目录内的所有文件上传到仓库根目录。
3. 打开仓库的 `Settings → Pages`。
4. 在 `Build and deployment` 中选择 `Deploy from a branch`。
5. 选择 `main` 分支和 `/(root)` 目录，然后保存。
6. 稍等片刻后访问 `https://你的用户名.github.io/resume/`。

## 修改内容

- 简历文字：编辑 `index.html`。
- 颜色和版式：编辑 `styles.css` 顶部的 CSS 变量。
- 头像：替换 `assets/headshot.jpg`，文件名保持不变。
- 手机和邮箱：在 `index.html` 的 `#contact` 区域修改。

网站已包含桌面端、平板和手机响应式布局、键盘可访问菜单、减少动态效果适配及打印样式。
