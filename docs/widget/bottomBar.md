# BottomNavigationBar尾部导航

> 底部导航条，可以很容易地在tap之间切换和浏览顶级视图。

```
bottomNavigationBar: BottomNavigationBar(
  items: <BottomNavigationBarItem>[
    BottomNavigationBarItem(icon: Icon(Icons.home), title: Text('Home')),
    BottomNavigationBarItem(icon: Icon(Icons.business), title: Text('Business')),
    BottomNavigationBarItem(icon: Icon(Icons.school), title: Text('School')),
  ],
  currentIndex: _selectedIndex,
  fixedColor: Colors.deepPurple,
  onTap: _onItemTapped,
  type: BottomNavigationBarType.fixed,
)
```

### 属性

- ## `type`
> 类型 BottomNavigationBarType： fixed   shifting

- ## `items`
> tab元素  icon： 图标     title: 标题

- ## `currentIndex`
> 当前选中目标 0开始

- ## `iconSize`
> 图标大小

- ## `fixedColor`
> 如果 type 类型为 fixed,则通过 fixedColor 设置选中 item 的颜色

# BottomNavigationBarItem

> - `icon`: 图标 widget,一般为 Icon 
> - `title`: 标题 widget,一般为 Text 
> - `backgroundColor`: item 的背景颜色
> - `activeIcon`: 选中图标 widget,一般为 Icon

**参考：**

[BottomNavigationBar](https://docs.flutter.io/flutter/material/BottomNavigationBar-class.html)