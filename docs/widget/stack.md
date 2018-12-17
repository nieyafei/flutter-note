# Stack层叠式布局

> 层叠布局和Web中的绝对定位、Android中的Frame布局是相似的, 允许子widget堆叠

- ## `alignment`

> 定如何去对齐没有定位（没有使用Positioned）或部分定位的子widget
> AlignmentDirectional:
> - AlignmentDirectional.

- ## `textDirection`

> 决定alignment对齐的参考系, 即：
> - textDirection的值为**TextDirection.ltr**，则alignment的start代表左，end代表右；
> - textDirection的值为**TextDirection.rtl**，则alignment的start代表右，end代表左。

- ## `fit`

> 决定没有定位的子widget如何去适应Stack的大小
> - **StackFit.loose**: 使用子widget的大小
> - **StackFit.expand**: 扩伸到Stack的大小

- ## `overflow`

> 如何显示超出Stack显示空间的子widget
> - **Overflow.clip**: 超出部分会被剪裁（隐藏）
> - **Overflow.visible**: 超出的部分不会隐藏


**原文链接：**

[层叠布局](https://book.flutterchina.club/chapter4/stack.html)

[Stack class](https://docs.flutter.io/flutter/widgets/Stack-class.html)