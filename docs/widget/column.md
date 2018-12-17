# Column线性布局

> 沿垂直方向排列其子widget

#### 属性：

- ## `children`

> 子内容, 子Widgets数组

```
Column(
  children: <Widget>[
    const FlutterLogo(),
    const Expanded(
      child: Text('hello world'),
    ),
    const Icon(Icons.sentiment_very_satisfied),
  ],
)
```

- ## `textDirection`

> 垂直方向子widget的布局顺序(是从上往下还是从下往上)

- ## `mainAxisSize`

> Row在主轴(水平)方向占用的空间，默认是`MainAxisSize.max`, `MainAxisSize.min`表示尽可能少的占用水平空间

- ## `mainAxisAlignment`

> 子Widgets在Column所占用的垂直空间内对齐方式, （mainAxisSize：MainAxisSize.max有效）

> MainAxisAlignment:
> - MainAxisAlignment.start: 沿textDirection的初始方向对齐, 若textDirection取值为TextDirection.ltr时，则MainAxisAlignment.start表示上对齐，textDirection取值为TextDirection.rtl时表示从下对齐
> - MainAxisAlignment.end: 与`start`相反
> - MainAxisAlignment.center: 垂直居中对齐

- ## `verticalDirection`

> Column横轴（水平）的对齐方向，默认是VerticalDirection.down，表示从左到右

- ## `crossAxisAlignment`

> 子Widgets在横轴方向的对齐方式
> CrossAxisAlignment:
> - CrossAxisAlignment.start: 左边对齐
> - CrossAxisAlignment.end: 右边对齐
> - CrossAxisAlignment.center: 居中对齐
> - CrossAxisAlignment.baseline: 子控件的baseline在交叉轴方向对齐
> - CrossAxisAlignment.stretch: 完全填充

**注意：**
> 如果Column里面再嵌套Column，那么只有对最外面的Column会占用尽可能大的空间，里面Column所占用的空间为实际大小，