# ListTile
> 一个固定高度的行，通常包含一些文本，以及一个行前或行尾图标。

```
ListTile(
  leading: const Icon(Icons.flight_land),
  title: const Text('Trix\'s airplane'),
  subtitle: _act != 2 ? const Text('The airplane is only in Act II.') : null,
  enabled: _act == 2,
  onTap: () { /* react to the tile being tapped */ }
)
```

### 属性

- ## `leading`
> title前面的Widget

- ## `title`
> 标题文字

- ## `subtitle`
> 子标题文字

- ## `enabled `
> 是否可以点击

- ## `selected`
> 选中状态

- ## `trailing`
> 右侧widget

- ## `isThreeLine `
> 是否三行显示的限制

- ## `onLongPress`
> 

**参考：**

[ListTile class](https://docs.flutter.io/flutter/material/ListTile-class.html)