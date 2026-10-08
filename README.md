# Kai Liu | 刘锴

个人学术主页，包含个人简介、研究方向和论文列表。页面与图片来自已有主页，保留原有内容和视觉样式。

这是一个纯静态网站，使用 HTML 和 CSS，无需安装前端依赖或执行构建。

## 文件结构

| 文件或目录 | 用途 |
| --- | --- |
| `index.html` | 首页内容、论文列表和链接 |
| `assets/css/style.css` | 页面样式和移动端布局 |
| `assets/images/` | 个人照片和论文图片，包含原始照片备份 |
| `.nojekyll` | 让 GitHub Pages 直接发布静态文件 |
| `.gitignore` | 排除本地临时文件 |

## 本地预览

在项目根目录运行：

```bash
python3 -m http.server 8000
```

打开 <http://localhost:8000>。也可以直接用浏览器打开 `index.html`。

## GitHub 仓库

源码保存在 [KaiLiu18/kailiu18.github.io](https://github.com/KaiLiu18/kailiu18.github.io)。`index.html`、`assets/` 和 `.nojekyll` 位于仓库根目录，GitHub Pages 可以直接发布，无需构建。

## 发布到 GitHub Pages

在仓库中发布主页：

1. 打开仓库的 **Settings → Pages**。
2. 在 **Build and deployment → Source** 选择 **Deploy from a branch**。
3. 选择分支 **main** 和目录 **/(root)**，点击 **Save**。
4. 在 Pages 设置中查看实际发布地址。

此仓库是用户主页仓库，发布地址为 <https://kailiu18.github.io/>。

## 修改主页

- 个人简介、研究方向和论文信息：编辑 `index.html`。
- 字号、颜色、布局和移动端样式：编辑 `assets/css/style.css`。
- 更换照片或论文图片：放入 `assets/images/`，更新对应的 `src` 路径。
- 添加论文：参考已有 `<article class="publication">` 区块，并为标题等元素使用新的、唯一的 `id`。

所有站内资源使用相对路径，也可以放在普通项目仓库下作为项目主页发布。

## 参考

- [创建 GitHub Pages 站点](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [配置 GitHub Pages 发布源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
