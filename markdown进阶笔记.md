# Markdown 进阶笔记
Markdown 不是排版软件，而是一层“纯文本 → 结构 → 样式”的约定,是轻量级标记语言
## 一、底层原理
- 解析器分两步：先按行做块级解析，用空行、缩进和行首符号搭出标题、段落、列表、代码块的骨架
- 再对每个叶子块做行内解析，处理强调、链接、代码。结果是一棵 AST，再由渲染器变成 HTML、PDF 或网页。
- 同一份源码换个渲染器就可能变样：表格、公式、脚注都是“方言”
## 二、编辑器
编辑器是一套工具链，好用的功能不只是预览。命令面板（Ctrl+Shift+P / Ctrl+P）让人不用背快捷键,多光标、列表自动续行、表格 Tab 跳格适合批量整理,粘贴图片自动落盘、代码高亮等，以下为主流markdown编辑器:
   1.Typora
• 所见即所得标杆，界面极简、即时渲染。
• 支持表格、公式、流程图、主题自定义。
• $14.99 一次性买断。
• 适合大量写作用户。
   2.MarkText（开源免费）
• Typora 免费替代品，实时渲染、界面简洁。
• 功能略少、更新较慢。
   3.VS Code（免费）
• 配合 Markdown All in One、Preview Enhanced 插件非常强大。
• 集成 Git、终端、AI 辅助。
• 适合开发者一体化工作流。
   4.Obsidian
• 双向链接、关系图谱、1000+ 插件、Canvas。
• 本地 Markdown 文件存储，隐私友好。
• 适合长期构建知识库。
   5.Logseq（开源）
• 大纲式笔记、双链、白板。
• 本地优先，适合结构化知识管理。
   6.HackMD
• 类 Google Docs 的多人实时协作 Markdown。
• 支持 LaTeX、UML、幻灯片导出。
   7.Notion
• 虽非纯 Markdown，但支持部分语法，协作体验优秀。
   8.mdview（2MB）
• 双击秒开、专注查看，Pro 版支持轻量编辑。
• 适合日常快速阅读 README、文档。
   9.ErgeMD（极速阅读器）
• 毫秒级打开速度，适合纯查看场景。
## 三、局限
Markdown 只描述结构，不描述数据、位置、笔迹、版面和权限。一旦笔记的核心信息落在这些维度上，它就开始别扭：
笔记类型	局限	更合适的工具
```

数据、台账	不能排序、筛选、汇总	Notion 数据库、Bases、Excel
白板、导图	没有位置和连线	Canvas、Excalidraw、Heptabase
手写、批注	没有笔迹、页码、高亮	GoodNotes、OneNote、Zotero
多人评审	没有评论、修订、权限	飞书、Word、HackMD
长论文、书	没有交叉引用和自动编号	LaTeX、Typst、Quarto
简历、海报、PPT	没有分栏和精细版面	Figma、Canva、PowerPoint
```


