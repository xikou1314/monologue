## 常见的定位方案

* 普通流

  > 在普通流中，元素按照其在HTML中的先后顺序至上而下布局，在这个过程中，行内元素水平排列，直到当行被占满然后换行，块级元素则会被渲染为完整的一个新行，除非另外指定，否则所有的元素默认都是普通流定位，也可以说，普通流中元素的位置由该元素在HTML文档中的位置决定

* 浮动

  > 在浮动布局中，元素首先按照普通流的位置出现，然后根据浮动的方向尽可能的向左边或右边偏移，其效果与印刷排版中的文本环绕相似

* 绝对定位

  > 在绝对定位布局中，元素会整体脱离普通流，因此绝对定位元素不会对其兄弟元素造成影响，而元素具体的位置由绝对定位的坐标决定

## BFC概念

BFC即Block Formatting Contexts(块级格式上下文)，它本身属于上文定义的普通流

**具有BFC特性的元素可以看作是隔离了的独立容器，容器里面的元素不会在布局上影响到外面的元素，并且BFC具有普通容器所没有的一些特性**

## 触发BFC

元素只要满足下面任一条件即可出发BFC特性

* body根元素
* 浮动元素：float除none以外的值
* 绝对定位元素：position(absolute、fixed)
* display为inline-block、table-cells、flex
* Overflow除了visible以为的值(hidden、auto、scroll)

## BFC特性

* 同一BFC下外边距会发生折叠

  > 可将发生折叠的元素放入不通的BFC中

* BFC可以包裹浮动元素(清除浮动)

* BFC可以阻止元素被浮动元素遮挡

  > 可以借此实现左列宽度固定，右列自定义宽度布局

## 参考

[10 分钟理解 BFC 原理](https://zhuanlan.zhihu.com/p/25321647)