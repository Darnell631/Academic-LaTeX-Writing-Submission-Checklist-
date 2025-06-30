# 📄 Academic LaTeX 写作 & 投稿全流程清单

![banner](https://img.shields.io/badge/LaTeX-Ready-blue?style=for-the-badge&logo=latex&logoColor=white)
![badge](https://img.shields.io/badge/ICML%2FNeurIPS%2FCVPR-Submission%20Checklist-green?style=for-the-badge&logo=overleaf)
![badge](https://img.shields.io/badge/中文版本-Supported-orange?style=for-the-badge)

> ✨ 一份系统、专业、现代的写作 & 投稿最终核对清单，适用于学术顶会与顶刊（ICML, NeurIPS, CVPR 等），帮你全面提高论文质量与接收率。

---

## 🚀 快速开始

✅ 逐项打勾，确保内容完整、排版专业、审稿人友好  
📌 兼容 LaTeX、Overleaf、VS Code + Markdown 等多种写作环境  
🎨 内含美观 icon、配色、图表风格建议，方便直接引用

---

## 🗂️ 清单内容（完整中文版）

## 🗂️ Sec2. 相关工作（Related Work）

- [ ] ✅ 使用 **Related Work**，而非 "Related Works"
- [ ] ✅ 当作者是主语时使用 `\citet{}`（例如 “Smith et al. (2019) showed…”）
- [ ] ✅ 在括号中引用时（ICML, ICLR），使用 `\citep{}`（例如 “…如最近研究所示 \citep{smith2019, johnson2020}.”）
- [ ] ✅ 遵循「Authors et al. + 动词（过去式）」与「方法名 + 动词（现在式）」的写法
- [ ] ✅ 避免错误引号：`"Hello, World!”` → ```Hello, World!''`

---

## 💡 Sec3. 方法（Method）

### ✨ 间距和格式

- [ ] ✅ 控制 **间距**：使用 `\vspace(-1ex)`（相对单位，会随字体大小缩放），比用 cm 更方便

### 🔤 符号约定

- [ ] ✅ 用 `\top` 表示转置，代替 `^T`
- [ ] ✅ **向量和矩阵**：使用粗体（`\mathbf{x}`，`\mathbf{W}`）
- [ ] ✅ **集合或损失函数**：使用花体（`\mathcal{L}`）
- [ ] ✅ 若有代数结构可用哥特体（`\mathfrak{g}`，$\mathfrak{g}$）
- [ ] ✅ 随机变量或分布可用无衬线字体（`\mathsf{X}`，$\mathsf{X}$）
- [ ] ✅ 范数书写规范：$\| x \|$ 而非 $||x||$
- [ ] 🔗 参考：完整 LaTeX 数学速查表 [查看这里](https://zhuanlan.zhihu.com/p/522724800)
- [ ] ✅ 最终检查：每个符号第一次出现时需明确定义（可内联或单独符号表）
- [ ] ✅ 最终检查：符号大小写保持一致（例如，不混用 $x$ 和 $X$ 除非有明确说明）

### 🧮 方程

- [ ] ✅ 方程若为句子一部分，末尾加标点（逗号或句号）
- [ ] ✅ 重要方程应编号（如 `\label{eq:loss}`）
- [ ] ✅ 多行方程使用 `align` 或 `alignat`
- [ ] ✅ 子脚注文字用 `\mathrm{}` 或 `\text{}`（如 $\mathcal{L}_{match}$ ⇒ `\mathcal{L}_{\mathrm{match}}`）
- [ ] ✅ 显示数学后继续正文可用 `\noindent` 避免缩进（例如 where ...）

### 📄 短小分节或伪标题

- [ ] ✅ 使用 `\noindent \textbf{Section Name.}` 形式书写小段落内伪分节

---

## 🔬 Sec4. 实验（Experiments）

### 🗺️ 流程图与示意图

- [ ] ✅ 字体使用 `Google Sans`，字号 > 25 pt
- [ ] ✅ 检查图例、标注和线条风格是否统一

### 🎨 调色方案

- [ ] ✅ **图表颜色**：为自己的方法选择明亮、突出的颜色
- ![image.png](image.png)
- ![image.png](image%201.png)
- ![image.png](image%202.png)
- ![image.png](image%203.png)
- [ ] ✅ **流程图颜色**：注意色盲友好（避免纯红-绿对比）
- ![image.png](image%204.png)
- ![image.png](image%205.png)
- ![image.png](image%206.png)
- [ ] ✅ **最终检查**：方法名一致、拼写无误、补充必要的小图例解释

### 📊 图表

- [ ] ✅ 图注放下方，表注放上方
- [ ] ✅ 使用 `Figure~\ref{fig:example}` 或 `Table~\ref{tab:example}`，避免写 “the figure below”
- [ ] ✅ 数字格式保持一致（如 0.40 而非 0.4）
- [ ] ✅ 每个注释至少两行，包含核心解释、数据集、backbone 或消融背景
- [ ] ✅ 轴标签清晰，含单位
- [ ] ✅ 使用矢量图（PDF、SVG、TikZ），避免位图
- [ ] ✅ **最终检查**：所有图表需在正文中被引用

---

## 📚 参考文献（References）

- [ ] ✅ 使用 dblp（[https://dblp.org/](https://dblp.org/)）获取准确引用，避免重复
- [ ] ✅ 严格遵循会议/期刊特定格式
    - [ ] 📄 **会议**：
        - [ ] Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)
        - [ ] CVPR（若页面受限可简写）
    - [ ] 📄 **期刊**：用全称（如 IEEE Transactions on Neural Networks and Learning Systems），包含卷号、期号、页码、年份

---

## 📂 附录 & 补充材料

- [ ] ✅ 包含 **目录**，若附录较大
- [ ] ✅ 在正文中显式引用附录
- [ ] ✅ 若为双盲审稿，需移除任何可识别身份信息（如日志、**docx** 文件）

---

## ✅ 提交前最终核对

- [ ] ✅ 所有 `\label{}` 与 `\ref{}` 已解决（无 "??"）
- [ ] ✅ 清除 PDF 元数据（不含个人信息）
- [ ] ✅ 全文拼写检查（可用 Grammarly 或 LanguageTool）
- [ ] ✅ 严格遵循页数限制（包括附录）

---

## 💬 联系与贡献

🤝 欢迎提出 PR 或 Issue，补充额外细节、图例模板或常见 reviewer 建议  
📧 有任何疑问或想交流更多写作经验，可通过 Issues 或 Discussions 与我联系

---

## 🌟 其他推荐

- ⭐ 使用 [Overleaf](https://www.overleaf.com/) 云协作写作
- 🟢 推荐工具：LanguageTool、Grammarly、Zotero
- 💻 建议版本管理：Git + Overleaf 同步

---

🎉 **完成所有核对后，恭喜你！论文离「接收」更近一步 🚀**

---

![footer](https://img.shields.io/badge/Good%20Luck%20%26%20Happy%20Writing-💪🎓-brightgreen?style=flat-square)
