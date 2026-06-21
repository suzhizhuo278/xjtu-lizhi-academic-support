# 高等数学IV-2 整合工程

这是从原始志愿者交付物整理出的干净 LaTeX 总工程。

## 文件结构

- `main.tex`：总入口。
- `chapters/chapter05.tex`：第五章，来自 `高数资料 (1).zip`。
- `chapters/chapter06.tex`：第六章，合并了 `高数资料 (1).zip` 的 6.1--6.3 和 `高数.zip` 的 6.4--6.8。
- `chapters/chapter07.tex`：第七章，由 Word 文档自动转写为 LaTeX 初稿。
- `chapters/chapter09.tex`：第九章，来自 `高数.zip`。
- `raw/`：保留未展开/未整合的小附件。

## 已知状态

- 当前使用 `高代封面.pdf` 作为占位封面。
- `mpdoc.sty` 中原本固定使用 `CMU Serif`，本机缺失该字体；本工程已改为优先使用 `CMU Serif`，缺失时回退到 `Latin Modern Roman`。
- 第七章由 Word 公式自动转换而来，建议人工复核公式和积分限。

## 编译

```bash
xelatex -interaction=nonstopmode -halt-on-error main.tex
```
