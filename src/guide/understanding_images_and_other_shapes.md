# 理解图片和其他形状

从概念上讲，Word 文档有两层，一个文本层和一个绘图层。 在文本层中，文本对象从左到右，从上到下流动，当前一页被填满时开始新的一页。 在绘图层中，称为形状的绘图对象放置在任意位置。 这些有时被称为浮动形状。

图片是可以出现在文本或绘图层中的形状。 当它出现在文本层中时，它被称为内嵌形状，或者更具体地说，是内嵌图片。

内联形状被视为大文本字符（字符字形）。 增加了行高以适应形状，并且形状被包裹成一条适合宽度方向的线，就像文本一样。 在它前面插入文本会导致它向右移动。 通常，图片单独放置在段落中，但这不是必需的。 它可以在放置它的段落中前后放置文本。

在撰写本文时，`python-docx` 仅支持内联图片。 可以添加浮动图片。 如果您有一个活跃的用例，请在问题跟踪器上提交功能请求。 `Document.add_picture()` 方法将指定图片添加到文档末尾的一段中。 但是，通过更深入地研究 API，您可以将文本放置在段落中图片的任一侧，或两者兼而有之。
