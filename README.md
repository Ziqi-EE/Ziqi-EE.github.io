# Ziqi-EE.github.io

这是 Song Ziqi 的个人学术主页，基于 GitHub Pages 和 Jekyll 构建，整体采用简洁的学术风格，内容与布局分离，方便后续持续更新。

## 目录结构

- `_layouts/`：页面整体模板。
- `_includes/`：导航栏、论文卡片、专利卡片等可复用组件。
- `_data/`：个人信息、研究方向、论文、专利、项目和导航数据。
- `assets/css/main.css`：全站样式与响应式布局。
- `assets/images/publications/` 与 `assets/images/patents/`：建议放置论文图片、图文摘要、专利附图。

## 内容更新

新增论文请编辑 `_data/publications.yml`，新增专利请编辑 `_data/patents.yml`。每条记录都支持 `image` 字段，可将图片放到对应目录后填写路径，例如：

```yml
image: "/assets/images/publications/example.jpg"
```

论文和专利展示区已经为每条记录预留左侧图片位置，后续添加图片时无需改动页面布局代码。

# 如果改动了任何东西 左侧这个分支会提示