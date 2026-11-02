# IELTS Listening Notes

雅思听力笔记 —— 独立仓库，与写作 Skills 仓库完全分离。

**站点地址**：https://huyushao521.github.io/ielts-listening/

## 当前内容

| 页面 | 说明 |
| --- | --- |
| `index.html` | 同义替换词汇：高频 / 中频 / 低频三档 + 同义替换技巧 |

## 目录结构

```
ielts-listening/
├── index.html          # 首页（同义替换词汇）
├── assets/
│   └── style.css       # 全站样式
└── README.md
```

## 本地预览

```powershell
python -m http.server 8000
# 打开 http://localhost:8000
```

## 如何扩充

新增栏目时，直接在本仓库根目录建独立 HTML 文件，并在 `index.html` 顶部导航 `nav-links` 里加一条链接即可。建议命名：

- `scenario-vocab.html` — 场景词汇（租房 / 校园 / 旅游 / 医疗等）
- `map-diagram.html` — 地图题与流程图题专项
- `numbers-spelling.html` — 数字、日期、拼写易错点
- `cambridge-review.html` — 剑雅真题复盘

样式统一复用 `assets/style.css`，页面骨架可直接复制 `index.html`。

## License

MIT
