- Bootstrap引入
```html
<!DOCTYPE html>
<html lang="zh-cn">
<head>
    <meta charset="UTF-8">
    <!-- 屏幕和设备的屏幕一致，初始缩放为1:1，禁止用户缩放 -->
    <meta name="viewport" content="width=device-width,initial-scale=1,user-scalable=no">
    <title>Document</title>
    <!-- 引入外部的bt中的css文件 -->
    <link rel="stylesheet" href="bootstrap/css/bootstrap.css">
    <!-- 必须先引入jq之后再引入js -->
    <script src="bootstrap/js/jquery.min.js"></script>
    <!-- 再引入bt.js文件 -->
    <script src="bootstrap/js/bootstrap.min.js"></script>
</head>
```
- span1/2/3/4

- ul.unstyled

- ul.inline

- 描述 `<dl> > <dt> > <dd>`

- 响应式导航条

- Glyphicons `<span>或者<a>`

- 动态模态对话框

- 滚动监听

- 工具提示框

- 弹出框

- 状态按钮
> 加载中...

- 折叠

- 幻灯

- 视频响应式
```html
<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="iqiyi.catilog2015/24551221.swf"></iframe>
</div>
```

- 扁平化风格页面

- 

- aria-expanded="false"
> aria-expanded表示展开状态。默认为undefined, 表示当前展开状态未知。其它可选值：true表示元素是展开的；false表示元素不是展开的。

- aria-hidden字符串
> 可选值为true和false,true表示元素隐藏(不可见)，false表示元素可见。
