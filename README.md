# portfolio-prototypes

产品原型作品集 —— 墨刀（MockingBot）导出的离线可交互演示包。

## 在线演示

👉 **https://loveilouise.github.io/portfolio-prototypes/**

点击上方链接即可直接在浏览器中打开原型，支持页面跳转、点击热区等完整交互，无需安装任何软件。

## 本地查看

由于原型的资源通过相对路径加载，直接双击 `index.html` 可能会因浏览器跨域策略而白屏。请用本地服务器打开：

```bash
# 在项目根目录执行
python -m http.server 8000
# 然后浏览器访问 http://localhost:8000
```

## 目录结构

| 路径 | 说明 |
| --- | --- |
| `index.html` | 原型入口页 |
| `env/` | 运行时环境配置 |
| `extra/` | 原型页面数据（`data.*.js`） |
| `mb-workspace/` | 墨刀播放器运行时（JS / CSS / 字体） |
| `mb-static/` | 静态资源（图标、兼容库） |
| `uploads4/`、`uploads5/`、`uploads6/` | 原型中使用的图片素材 |

## 技术说明

- 纯静态站点，通过 GitHub Pages 托管（源为 `main` 分支根目录）
- 根目录的 `.nojekyll` 用于关闭 GitHub Pages 的 Jekyll 构建，确保所有静态资源原样发布
