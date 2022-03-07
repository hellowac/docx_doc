# 风格行为

除了收集一组格式属性之外，样式还有五个指定其行为的属性。这种行为比较简单，基本上相当于样式出现在 `Word` 或 `LibreOffice UI` 中的时间和位置。

理解风格行为的关键概念是推荐列表。在 `Word` 的样式窗格中，用户可以选择他们想要查看的样式列表。其中之一被命名为推荐并且被称为推荐列表。所有五个行为属性都会影响此列表和样式库中样式外观的某些方面。

简而言之:

如果一个样式的 `hidden` 属性为 `False`（默认值），它就会出现在推荐列表中。

如果样式未隐藏且其 `quick_style` 属性为 `True`，则它也会出现在样式库中。

如果隐藏样式的 `unhide_when_used` 属性为 `True`，则其隐藏属性在第一次使用时设置为 `False`。

样式列表和样式库中的样式按优先级排序，然后按字母顺序排列相同优先级的样式。

如果样式的`locked`属性为 `True` 并且为文档打开了格式限制，则该样式将不会出现在任何列表或样式库中，并且不能应用于内容。