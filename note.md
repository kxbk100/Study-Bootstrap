- Bootstrap引入
```html
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>贴吧后台管理页面</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
    <script src="../js/jquery.min.js"></script>
    <script src="../js/bootstrap.min.js"></script>
</head>

<body>
    <!-- 页眉 -->
    <header>
        <!-- 导航条部分 -->
        <nav>
            ...
        </nav>
    </header>
    <!-- 主要内容 -->
    <div class="container">
        <div class="row">
            <!-- 左侧目录 -->
            <div class="col-xs-12 col-sm-2 col-md-2 col-lg-2">
                ...
            </div>
            <!-- 右侧主要内容 -->
            <div class="col-xs-12 col-sm-10 col-md-10 col-lg-10">
                ...
            </div>
        </div>
    </div>
    <!-- 页尾 -->
    <footer>
        ...
    </footer>
</body>

</html>
```
- 制作一个页面的流程
> - 引入框架
> - 实现页面布局代码
> - 构建导航的整体架构
> - 设计标题和导航链接
> - 设计搜索框和通知系统
> - 设置管理员登录系统
> - 设计响应式导航
> - 左侧边栏设计
> - 页面主体设计

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

- 各种风格的按钮

- jQuery插件 DataTables响应式表格
> 支持及时分页、搜索、排序

> Json、数组、Ajax

- 可视化图表ECharts

- jQuery UI Bootstrap工具

- aria-expanded="false"
> aria-expanded表示展开状态。默认为undefined, 表示当前展开状态未知。其它可选值：true表示元素是展开的；false表示元素不是展开的。

- aria-hidden字符串
> 可选值为true和false,true表示元素隐藏(不可见)，false表示元素可见。

- 快捷键
> - Ctrl+Shift+Enter 在上一行另起一行
> - Ctrl+Enter 光标不在末尾回车
> - Ctrl+Backspace 删除一个词

-  col-xs-n中放图片不生效
```css
img {
	display: block;
	max-width: 100%;
}
```
- display
> - block   此元素将显示为块级元素，此元素前后会带有换行符
> - inline  默认。此元素会被显示为内联元素，元素前后没有换行符|
> - inline-block    行内块元素。（CSS2.1 新增的值）

- 使用col就要在母元素上清除浮动，因为col栅格也是浮动的
使用flag覆盖叠加新的属性 css中使用```css.side-bar-card.flag {}```来调用，html中用```html<div class="side-bar-card flag clearfix">```

- a标签链接不带下划线，并列换行写
```css
a,
a:hover,
a:visited,
a:link,
a:active {
    text-decoration: none;
}
```

- line-heigh不要写px

- 表格居中
```html
<table align="center">
```

- bootstrap响应式表格
```html
<div class="table-responsive">
```
- 表格内容水平垂直居中
```html
<th style='text-align: center;'>host</th>   水平居中
<td rowspan=$row_host1 style='vertical-align: middle;'>host1</td>   垂直居中
<td rowspan=$rowspan style='vertical-align: middle;text-align: center;'>hello</td>  既水平又垂直居中
```

- 图片撑满
```css
background-size: cover;
```
- 数据不为空显示
```html
<if condition="$result[0]['jiyao_id'] neq null">
	<tr>
        <td style="vertical-align: middle;text-align:center;width: 20%">
            <span><b>机要编号</b></span>
        </td>
        <td class="description">{$result[0]['jiyao_id']}</td>
    </tr>
</if>
```

- 1 0转换
```html
<if condition="$student.is_searched eq 1">已查询<else/>未查询</if></td>
```

- thinkphp无法访问
> 可能保存了带bom的utf编码

- thinkphp部署到iis服务器
> 将runtime设定到支持写入的目录

- input/select/textarea/... + .form-control

- .form-group
> 单独的表单控件会被自动赋予一些全局样式。所有设置了`.form-control`类的`<input>、<textarea>和<select>`元素都将被默认设置宽度属性为`width: 100%;`。将`label`元素和前面提到的控件包裹在`.form-group`中可以获得最好的排列

- 响应式表格
> 将任何 .table 元素包裹在`<div class="table-responsive">`元素内

- 垂直方向的内容截断
> 响应式表格使用了 overflow-y: hidden 属性，这样就能将超出表格底部和顶部的内容截断。特别是，也可以截断下拉菜单和其他第三方组件

- .form-inline
> - 输入框和单选/多选框控件默认被设置为 width: 100%; 宽度。在内联表单，我们将这些元素的宽度设置为 width: auto;，因此，多个控件可以排列在同一行。根据布局需求，手动设置宽度
> - 一定要添加 label 标签，对于内联表单，可以通过为label设置.sr-only类将其隐藏。还有一些辅助技术提供label标签的替代方案，比如 aria-label、aria-labelledby 或 title 属性

- .form-horizontal
> 无需再添加.row了

- margin对span无效
> - display:block;
> - line-height

- button后退
```html
<button class="btn btn-danger ycx" onclick="javascript :history.back(-1);">返回</button>
```

- 居中
> - 文本内容居中：text-center
> - 图片居中：center-block
> - 其他类型元素居中：col-md-offset-X

