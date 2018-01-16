BFC就是这样的东西:

1. 它没有定义
2. 它只有特性/功能

浮动，绝对定位元素，非块盒的块容器（例如，inline-blocks，table-cells和table-captions）和'overflow'不为'visible'的块盒会为它们的内容建立一个新的块格式化上下文;

BFC元素特性表现原则就是，内部子元素再怎么翻江倒海，翻云覆雨都不会影响外部的元素。

### 功能1： 爸爸管儿子

用BFC包住浮动元素（这不是清浮动，clearfix才是）。

### 功能2：兄弟之间划清界限

用float+div做左右自适应布局。

### 功能3：解决margin合并问题


备注：

display:flow-root 是最纯粹的创建BFC的方法。

没有任何情况是一定要使用BFC的，除了面试。