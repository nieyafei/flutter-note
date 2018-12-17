# Container容器组件

> 相当于HTML里的`<div>`标签

```
Center(
  child: Container(
    margin: const EdgeInsets.all(10.0),
    color: const Color(0xFF00FF00),
    width: 48.0,
    height: 48.0,
  ),
)
```
#### 属性：

- ## `Alignment`

> 容器子内容的对齐方式
> - bottomCenter:下部居中对齐。
> - botomLeft: 下部左对齐。
> - bottomRight：下部右对齐。
> - center：纵横双向居中对齐。
> - centerLeft：纵向居中横向居左对齐。
> - centerRight：纵向居中横向居右对齐。
> - topLeft：顶部左侧对齐。
> - topCenter：顶部居中对齐。
> - topRight： 顶部居左对齐。

- ## `child`

> 子内容

- ## `width`

> 容器宽度（ep: 500.0）

- ## `height`

> 容器高度（ep: 500.0）

- ## `color`

> 容器背景颜色

- ## `margin`

> 容器外补白

- ## `padding`

> 容器内补白

- ## `transform`

> 容器变换

- ## `constraints`

> 容器大小的限制条件

```
  BoxConstraints({
    double minWidth: 0.0, 
    double maxWidth: double.infinity, 
    double minHeight: 0.0, 
    double maxHeight: double.infinity 
  })
```

- ## `decoration`

> 背景装饰

- ## `foregroundDecoration`

> 前景装饰

**注意：**

> 容器的大小可以通过`width`、`height`属性来指定，也可以通过`constraints`来指定，如果同时存在时，width、height优先。实际上Container内部会根据width、height来生成一个constraints。

> `color`和`decoration`是互斥的，实际上，当指定color时，Container内会自动创建一个decoration。