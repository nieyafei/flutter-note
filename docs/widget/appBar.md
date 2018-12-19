# AppBar
> 典型的AppBar，带有标题、操作和溢出的下拉菜单。

```
AppBar({
  Widget leading, 
  bool automaticallyImplyLeading: true, 
  Widget title, 
  List<Widget> actions, 
  Widget flexibleSpace, 
  PreferredSizeWidget bottom, 
  double elevation: 4.0, 
  Color backgroundColor, 
  Brightness brightness, 
  IconThemeData iconTheme, 
  TextTheme textTheme, 
  bool primary: true, 
  bool centerTitle, 
  double titleSpacing: NavigationToolbar.kMiddleSpacing, 
  double toolbarOpacity: 1.0, 
  double bottomOpacity: 1.0 
})
```

### 属性：

![image](../images/appbar/app_bar.png ':no-zoom')

- ## `leading`
> 标题前面的Widget

- ## `automaticallyImplyLeading`
> 

- ## `title`
> 标题, 通常显示为当前界面的标题文字

- ## `actions`
> Widget 列表，代表 Toolbar 中所显示的菜单

- ## `flexibleSpace`
> 一个显示在 AppBar 下方的控件，高度和 AppBar 高度一样，可以实现一些特殊的效果，该属性通常在 SliverAppBar 中使用

- ## `bottom`
> 一个 AppBarBottomWidget 对象，通常是 TabBar

- ## `elevation`
> 纸墨设计中控件的 z 坐标顺序，默认值为 4，对于可滚动的 SliverAppBar，当 SliverAppBar 和内容同级的时候，该值为 0， 当内容滚动 SliverAppBar 变为 Toolbar 的时候，修改 elevation 的值

- ## `backgroundColor`
> APP bar 的颜色，默认值为 ThemeData.primaryColor

- ## `brightness`
> App bar 的亮度，有白色和黑色两种主题，默认值为 ThemeData.primaryColorBrightness

- ## `iconTheme`
> App bar 上图标的颜色、透明度、和尺寸信息。默认值为 ThemeData.primaryIconTheme

- ## `textTheme`
> App bar 上的文字样式。默认值为 ThemeData.primaryTextTheme

- ## `centerTitle`
> 标题是否居中显示，默认值根据不同的操作系统，显示方式不一样

- ## `primary`
> 是否默认样式

- ## `titleSpacing`
> 标题两边的空白区域

- ## `toolbarOpacity`
> 整个导航栏的不透明度

- ## `bottomOpacity`
> bottom内容的不透明度

**参考：**

[AppBar 基础](https://flutterchina.club/catalog/samples/basic-app-bar/)

[AppBar class](https://docs.flutter.io/flutter/material/AppBar-class.html)