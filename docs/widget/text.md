# Text文本组件

```
class MyApp extends StatelessWidget{
  @override
  Widget build(BuildContext context ){
      return MaterialApp(
        title:'Text文本组件',
        home:Scaffold(
          body:Center(
            child:new Text('Hello World')
          ),
        ),
      );
  }
}
```
#### 属性：

- ## `TextAlign`

> 文本的对齐方式
> - center: 文本以居中形式对齐,这个也算比较常用的了。
> - left:左对齐，经常使用，让文本居左进行对齐，效果和start一样。
> - right :右对齐，使用频率也不算高。
> - start:以开始位置进行对齐，类似于左对齐。
> - end: 以为本结尾处进行对齐，不常用。有点类似右对齐.

- ## `maxLines`

> 设置最多显示的行数   number类型

- ## `overflow`

> 设置文本溢出

> - **clip**：直接切断，剩下的文字就没有了
> - **ellipsis**:在后边显示省略号，体验性较好
> - **fade**: 溢出的部分会进行一个渐变消失的效果，当然是上线的渐变，不是左右渐变。

- ## `style`

> 设置Text样式, TextStyle:
> - **background**: 背景色
> - **color**: 颜色
> - **debugLabel**: 调试标记
> - **decoration**: 添加上划线，下划线，删除线
> - **decorationColor**: 划线的颜色
> - **decorationStyle**: style可能控制画实线，虚线，两条线，点, 波浪线等
> - **fontFamily**: 字体
> - **fontSize**: 字大小
> - **fontStyle**: 文本显示样式
> - **fontWeight**: 字体粗重权重
> - **foreground**: 文本的前景色，不能与color共同设置
> - **hashCode**
> - **height**: 行高
> - **inherit**: true/false  是否继承默认样式
> - **letterSpacing**: 单词之间的间距
> - **locale**: 国际化
> - **shadows**: 阴影
> - **textBaseline**: 基线
> - **wordSpacing**: 字母之间的间距

```
Text(
  'Hello World',
  style: TextStyle(
    fontWeight: FontWeight.bold,
    color: Colors.black
  ),
)
```

# RichText

> 富文本Text，可以显示多种样式的text

```
RichText(
  text: TextSpan(
    text: 'Hello ',
    style: DefaultTextStyle.of(context).style,
    children: <TextSpan>[
      TextSpan(text: 'bold', style: TextStyle(fontWeight: FontWeight.bold)),
      TextSpan(text: ' world!'),
    ],
  ),
)
```

# DefaultTextStyle

> 文字样式，用于指定Text widget的文字样式

```
DefaultTextStyle({
  @required TextStyle style, 
  TextAlign textAlign, 
  bool softWrap: true, 
  TextOverflow overflow: TextOverflow.clip, 
  int maxLines,
})
```

**widget树中，文本的样式默认是可以被继承的，因此，如果在widget树的某一个节点处设置一个默认的文本样式，那么该节点的子树中所有文本都会默认使用这个样式，而DefaultTextStyle正是用于设置默认文本样式的**

**参考：**

[Flutter中文](https://book.flutterchina.club/chapter3/text.html)

[Flutter: Text Class](https://docs.flutter.io/flutter/widgets/Text-class.html)

[Flutter: RichText](https://docs.flutter.io/flutter/widgets/RichText-class.html)

[Flutter: DefaultTextStyle](https://docs.flutter.io/flutter/widgets/DefaultTextStyle-class.html)

**欢迎大家一起补充**
