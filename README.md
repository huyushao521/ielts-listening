# IELTS Listening Notes

雅思听力笔记 —— 独立仓库，与写作 Skills 仓库完全分离。

**站点地址**：https://huyushao521.github.io/ielts-listening/

## 页面

| 页面 | 说明 |
| --- | --- |
| `index.html` | 按真题集整理：剑雅 C4–C19 高频同义替换，支持关键词搜索 |
| `vocabulary.html` | 同义替换总表：高频 / 中频 / 低频三档 + 同义替换技巧 |

## 目录结构

```
ielts-listening/
├── index.html              # 首页：按真题集（数据驱动渲染）
├── vocabulary.html         # 同义替换总表
├── assets/
│   ├── style.css           # 全站样式
│   ├── data-15-19.js       # 剑雅 C15–C19 数据
│   ├── data-10-14.js       # 剑雅 C10–C14 数据
│   └── data-4-9.js         # 剑雅 C4–C9 数据
└── README.md
```

## 如何新增条目

编辑对应的 `assets/data-*.js`，在某一册的 `v` 数组里追加一行：

```js
["听力原文（听到）", "题目/选项（看到）", "S1", "说明/场景"]
```

保存后刷新页面即可，无需构建。新增一册时，按同样结构 push 一个对象到 `window.IELTS_BOOKS`。

## 本地预览

```powershell
python -m http.server 8000
# 打开 http://localhost:8000
```

## License

MIT
