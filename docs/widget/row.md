# Row线性布局

> 沿水平方向排列其子widget


#### 属性：

- ## `children`

> 子内容, 子Widgets数组

```
Row(
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

> 水平方向子widget的布局顺序(是从左往右还是从右往左), 默认为系统当前Locale环境的文本方向(如中文、英语都是从左往右，而阿拉伯语是从右往左)。

- ## `mainAxisSize`

> Row在主轴(水平)方向占用的空间，默认是`MainAxisSize.max`, `MainAxisSize.min`表示尽可能少的占用水平空间

- ## `mainAxisAlignment`

> 子Widgets在Row所占用的水平空间内对齐方式, （mainAxisSize：MainAxisSize.max有效）

> MainAxisAlignment:
> - MainAxisAlignment.start: 沿textDirection的初始方向对齐, 若textDirection取值为TextDirection.ltr时，则MainAxisAlignment.start表示左对齐，textDirection取值为TextDirection.rtl时表示从右对齐
> - MainAxisAlignment.end: 与`start`相反
> - MainAxisAlignment.center: 居中对齐

- ## `verticalDirection`

> Row纵轴（垂直）的对齐方向，默认是VerticalDirection.down，表示从上到下

- ## `crossAxisAlignment`

> 子Widgets在纵轴方向的对齐方式
> CrossAxisAlignment:
> - CrossAxisAlignment.start: 顶部对齐
> - CrossAxisAlignment.end: 底部对齐
> - CrossAxisAlignment.center: 居中对齐
> - CrossAxisAlignment.baseline: 子控件的baseline在交叉轴方向对齐
> - CrossAxisAlignment.stretch: 完全填充

**注意：**

> 如果Row里面嵌套Row，那么只有对最外面的Row会占用尽可能大的空间，里面Row所占用的空间为实际大小，