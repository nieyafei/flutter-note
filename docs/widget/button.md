# 按钮

## RaisedButton

> "漂浮"按钮，它默认带有阴影和灰色背景。按下后，阴影会变大

## FlatButton

> 扁平按钮，默认背景透明并不带阴影。按下后，会有背景色

## OutlineButton

> 有一个边框，不带阴影且背景透明。按下后，边框颜色会变亮、同时出现背景和阴影(较弱)

## IconButton

> 一个可点击的Icon，不包括文字，默认没有背景，点击后会出现背景

## 自定义按钮外观

```js
FlatButton({
  Key key, 
  @required VoidCallback onPressed, //按钮点击回调
  ValueChanged<bool> onHighlightChanged, 
  ButtonTextTheme textTheme, 
  Color textColor, // 按钮文字颜色
  Color disabledTextColor, // 按钮禁用状态下文字颜色
  Color color, // 按钮背景颜色
  Color disabledColor, // 按钮禁用状态下背景颜色
  Color highlightColor, // 按钮按下时的颜色
  Color splashColor, // 点击时，水波动画中水波颜色
  Brightness colorBrightness, // 按钮主体，默认浅色主题
  EdgeInsetsGeometry padding, // 按钮填充
  ShapeBorder shape, // 外形
  Clip clipBehavior: Clip.none, 
  MaterialTapTargetSize materialTapTargetSize, // 
  @required Widget child  // 内容
})
```


**参考：**

[Flutter: 按钮（中文）](https://book.flutterchina.club/chapter3/buttons.html)

[FlatButton class](https://docs.flutter.io/flutter/material/FlatButton-class.html)