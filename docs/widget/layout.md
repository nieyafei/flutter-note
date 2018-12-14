# layout布局

## Container
  > 一个拥有绘制、定位、调整大小的 widget

  ### 参数：
  
  - `constraints`：约束

  > constraints: new BoxConstraints.expend()

  ##### BoxConstraints：

  1、通过配置创建框架的约束
  ```
  BoxConstraints({
    double minWidth: 0.0, 
    double maxWidth: double.infinity, 
    double minHeight: 0.0, 
    double maxHeight: double.infinity 
  })
  ```
  2、创建配置填充其他框的约束

  ```
  BoxConstraints.expand({
    double width, 
    double height 
  })
  ```
  3、配置不超过框架大小的约束
  
  ```
  BoxConstraints.loose(Size size)
  ```

  4、配置框架大小的约束

  ```
  BoxConstraints.tight(Size size)
  ```

  5、配置固定的宽度和高度的约束

  ```
  BoxConstraints.tightFor({
    double width, 
    double height 
  })
  ```

  6、配置固定宽度或高度的框约束，除非它们是无限的

  ```
  BoxConstraints.tightForFinite({
    double width: double.infinity, 
    double height: double.infinity 
  })
  ```

  - `padding`：内边距

  - `color`：颜色

  - `alignment`: 对齐方式

  - `child`：子控件

  - `foregroundDecoration`：前置装饰

  - `transform`：转场方式

  ### 代码块
  
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

## Padding


## Center


## Align


## FittedBpx


## AspectRatio


## ConstrainedBox



## Baseline



## FractionallySizedBox


## IntrinsicHeight



## IntrinsicWidth


## LimitedBox


## Offstage


## OverflowBox


## SizedBox


## SizedOverflowBox


## Transform


## CustomSingleChildLayout


**文档：**
  
  [中文：布局 Widget](https://flutterchina.club/widgets/layout/)

  [原文：布局 Widget](https://flutter.io/docs/development/ui/widgets/layout)