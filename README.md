# TE LI 个人网站：Works / About

按 https://www.teli.es/works 和 https://www.teli.es/about 的页面内容及排版重构（2026-09-05）。

## 本地打开
解压后双击 index.html；通过顶部导航切换 Works 和 About。无需 npm、框架、构建工具或 Google Sites 账户。请保留 assets 文件夹与页面的相对位置。

## 文件说明
- index.html：默认首页，即 Works 页面，包含个人介绍、14 项作品与其他外部链接。
- about.html：News、作品集、研究经历、教育、论文、荣誉及工作/教学经历。
- style.css：两个页面共用样式；包含手机宽度下的排版规则。
- script.js：本地页面搜索。
- assets/：原站图片、作品集 PDF、动态打字及群体运动动画。

## 编辑与部署
直接编辑 HTML 中的文字、图片 src 和链接 href。Works 页面即 index.html，只需维护这一份。搜索内容存放于 script.js 开头的 siteSearch 数组，更新正文时可同步修改。

将本目录全部内容上传到任意静态网站服务器即可（例如 GitHub Pages、Netlify、Cloudflare Pages，或自己的服务器）。本次未修改域名、原站或发布配置。

如希望保留原来的 /works 与 /about 无扩展名地址，请在部署平台开启 clean URLs，或配置 /works → / 或 /index.html、/about → /about.html 的内部重写。页面导航使用 .html 相对链接，适用于本地打开及子目录部署。

## 保留与差异
保留原站的内容顺序、十二列布局比例、双列/三列作品区、留白、News 折叠及两处原有动画。移除 Google Sites 自带的追踪、编辑/举报界面；导航搜索改为本地页面关键词搜索。

已下载的 10 张图片与 PDF 均为本地资源；另 6 张图片依照你的要求保留占位，请按 IMAGE-GUIDE.md 在本地替换；外部论文、项目、Figma、绘画网站及联系表单链接仍需联网。PDF 预览外观取决于浏览器的内置阅读器，不再使用 Google Drive 阅读器；若嵌入预览不可用，点击 Open portfolio 单独打开。PDF 约 57 MiB，部署平台如有单文件上限，可将其另行托管，并修改 about.html 的两处 PDF 地址。

字体渲染、PDF 工具栏及不同设备的换行可能与 Google Sites 略有不同。已检查文本覆盖、已保存图片的文件有效性、占位图、相对资源链接和脚本语法；未执行本地浏览器逐像素对比。
