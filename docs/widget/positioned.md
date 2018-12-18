# Positioned层叠式布局

> 子widget定位（根据Stack的四个角）

```
Positioned({
  double left, 
  double top, 
  double right, 
  double bottom, 
  double width, 
  double height
})
```

#### 属性：
- ## `left`、`top` 、`right`、 `bottom`

> 分别代表离Stack左、上、右、底四边的距离

- ## `width`, `height`

> 用于配合left、top 、right、 bottom来定位widget

> - 水平方向时，你只能指定left、right、width三个属性中的两个，如指定left和width后，right会自动算出(left+width)
> - 垂直方向时，你只能指定top、bottom、height三个属性中的两个，如指定top和height后，bottom会自动算出(top+height)

**原文链接：**

[层叠布局](https://book.flutterchina.club/chapter4/stack.html)

[Positioned class](https://docs.flutter.io/flutter/widgets/Positioned-class.html)