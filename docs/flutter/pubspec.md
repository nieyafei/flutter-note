### pubspec.yaml文件的配置

- #### name: 包名

  > 包名： 如果修改了包名，则整个项目所引入的文件，引用前的包名都需要更改
  > **不要轻易更改**

- #### 插件dev_dependencies

  ```
  dev_dependencies:
    flutter_test:
      sdk: flutter

      english_words: ^3.1.0
      shared_preferences: ^0.4.2
  ```

- #### assets：图片资源引入

  ```
  ## 配置
  assets:
    - images/start.gif  
  ```

- #### 字体配置

  ```
  ## 可以自定义字体
    fonts:
    - family: Schyler
      fonts:
        - asset: fonts/Schyler-Regular.ttf
        - asset: fonts/Schyler-Italic.ttf
          style: italic
    - family: Trajan Pro
      fonts:
        - asset: fonts/TrajanPro.ttf
        - asset: fonts/TrajanPro_Bold.ttf
          weight: 700
  ```

- #### 国际化

  ```
  uses-material-design: true
  ```


