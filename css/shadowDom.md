Shadow DOM 允许将隐藏的 DOM 树附加到常规的 DOM 树中——它以 shadow root 节点为起始根节点，在这个根节点的下方，可以是任意元素，和普通的 DOM 元素一样。

* Shadow host：一个常规 DOM节点，Shadow DOM 会被附加到这个节点上。
* Shadow tree：Shadow DOM内部的DOM树。
* Shadow boundary：Shadow DOM结束的地方，也是常规 DOM开始的地方。
* Shadow root: Shadow tree的根节点。