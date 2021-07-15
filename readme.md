# 引入bootstrap

1. 下载源码
2. 通过npm安装
3. 使用cdn

# 使用bootstrap

```html
<linkrel="stylesheet"href="./dist/css/bootstrap.min.css">
    
    
<script src="./jQuery.js"></script>
<script src="dist/js/bootstrap.min.js"></script> 
```

# 布局

```html
  <div class="container" style="background-color:pink;">
       .container用于固定宽度并且支持响应式布局的容器
    </div>
    <div class="container-fluid" style="background-color:red ;">
        .container-fluid用于100%宽度，占据全部视口容器
    </div>
```

# 栅格

~~~html
  <!-- 栅格系统 -->
    <div class="container">
        <div class="row">
            <!-- 列元素 col-xs-num col-sm-num col-md-num col-lg-num -->
            <div class="col-md-3" style="background-color: pink;">4</div>
            <div class="col-md-8" style="background-color: plum;">8</div>
            <div class="col-md-9" style="background-color: purple;">9999</div>
        </div>
        ------------------------------------
        <!-- 列组合 -->
        <div class="row">
            <div class="col-md-6" style="background-color: royalblue;">66666666</div>
            <div class="col-md-6" style="background-color: sandybrown;">55555555555</div>
            <div class="col-md-1" style="background-color:springgreen;">44444444444</div>
        </div>
        --------------------------------------------------
         <!-- 列偏移 -->
        <div class="row-p">
            <div class="col-md-2 " style="background-color: rgb(19, 32, 73);">66666666</div>
            <div class="col-md-6 col-md-offset-1" style="background-color: rgb(46, 26, 117);">55555555555</div>
            <div class="col-md-1" style="background-color:rgb(18, 119, 69);">44444444444</div>
        </div>
        -----------------------------------------------
        <!-- 列排序 -->
        <div class="row">
            <div class="col-md-2 " style="background-color: rgb(19, 201, 192);">123</div>
            <div class="col-md-6 col-md-push-1" style="background-color: rgb(153, 160, 219);">456</div>
            <div class="col-md-1" style="background-color:rgb(226, 38, 94);">789</div>
        </div>
        ------------------------------------
        <!-- 列嵌套 -->
        <div class="row">
            <div class="col-md-6" style="background-color: tomato;">156
                <div class="row">
                    <div class="col-md-1 " style="background-color: turquoise;">
                            445
                    </div>
                    <div class="col-md-8 " style="background-color: turquoise;">
                        444
                </div>
                </div>
            </div>
        </div>
    </div>
~~~

![image-20210714160042623](https://i.loli.net/2021/07/14/rfbIkTxU8Rqzav5.png)

# 常用样式

 small标签可以添加副标题

  段落：可以通过.lead来突出强调内容

 ` <small>`小号字体

 `<b><strong>`：加粗

 `<i><em>`:斜体

## 强调

定义了一套类名，通过颜色来表示强调

.text-muted:提示，使用浅灰色

text-primary：主要，使用蓝色

text-success：成功，使用浅绿色

text-info：通知信息，使用浅绿色

text-warning：警告，使用黄色

text-danger：危险，使用褐色

## 对齐

text-left：左对齐

text-right：右对齐

text-center：中间对齐

text-justify：两端对齐

# 列表

无序列表

~~~html
<ul><li>.....</li></ul>
~~~



有序列表

~~~html
<ol><li>....</li></ol>
~~~

定义列表

~~~html
<dl><dt>...</dt><dd>...</dd></dl>
~~~

内联列表

~~~html
class = "list-inline"
去点列表
class = "list-unstyled"
~~~

# 表格

## 基础样式

.table :基础样式

## 附加样式

table-striped：斑马线表格

table-bordered：带边框的表格

table-hover：鼠标悬停时高亮

table-condensed：紧凑表格

# 表单

## 表单控件

.form-control 	input-lg	input-sm

输入框

~~~html
<div class="row">
    <div class="col-md-3">
        <input type="text" class="form-control "> 
    </div>
</div>
~~~

下拉选择

~~~html
<div class="row">
    <div class="col-md-3">
        <select name="" id="" class="form-control">
            <option value="">请选择城市</option>
            <option value="">北京</option>
            <option value="">天津</option>
            <option value="">河北</option>
        </select>
    </div>
</div>
~~~

文本域

~~~html
<div class="row">
    <div class="col-md-3">
            <textarea name="" id="" cols="30" rows="10" class="form-control"></textarea>
    </div>
</div>
~~~

选框

~~~HTML
<div class="container">
    <!-- 垂直显示 -->
        <div class="col-md-3">
            <div class="radio">
                <label for=""><input type="radio"/>男</label>
            </div>
            <div class="radio">
                <label for=""><input type="radio" />女</label>
            </div>
        </div>
        <!-- 水平方向 -->
        <div class="row">
            <div class="col-md-3">
                <label class="radio-inline">
                    <input type="radio" name="" id=""> 测试
                </label>
                <label class="radio-inline">
                    <input type="radio" name="" id=""> 测试
                </label>
                </div>
            </div>
        </div>
</div>
~~~

## 按钮

基础样式：btn

` <button class="btn">按钮</button>` 

附加样式

btn-primary

btn-info

btn-sucess

btn-warning

btn-danger

btn-link

btn-defualt

 ~~~html
   <button class="btn btn-anger">按钮</button>
     <button class="btn btn-primary">按钮</button>
     <button class="btn btn-info">按钮</button>
     <button class="btn btn-success">按钮</button>
     <button class="btn btn-default">按钮</button>
     <button class="btn btn-warning">按钮</button>
     <button class="btn btn-link">按钮</button>
     <button class="btn btn-anger">按钮</button>
 ~~~



