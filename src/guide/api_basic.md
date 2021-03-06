# API基础知识

[docx.api.Document]: ../api/document.md

python-docx 的 API 旨在使简单的事情变得简单，同时通过适度和增量的理解投入来实现更复杂的结果。

可以仅使用单个对象创建基本文档，即打开文件时返回的 [docx.api.Document] 对象。 [docx.api.Document] 上的方法允许将块级对象添加到文档的末尾。 块级对象包括段落、内嵌图片和表格。 标题、项目符号和编号列表只是应用了特定样式的段落。

通过这种方式，可以从上到下“编写”文档，大致就像一个人确切知道自己想说什么这个基本用例，内容总是添加到文档的末尾，预计可能占实际用例的 `80%`，因此在不影响整个 `API` 的功能的情况下使其尽可能简单是优先事项。

## 内联对象

[docx.api.Document] 上的每个块级方法，例如 `add_paragraph()`，返回创建的块级对象。 通常不需要参考； 但是当必须单独创建内联对象时，您将需要块级对象的引用来执行此操作。
