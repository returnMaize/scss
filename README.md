## 介绍

```
base 用来控制所有和size相关的基准
color 颜色相关变量
size size变量
generator 根据size base color生成类名
other 手写一些常用类名
```

## 使用

```
import './scss/index.scss'
```

## 类名

> 变量的取值可以在 variable.scss 中增删改查 num 代表的数值大小可以在 base.scss 中修改(默认都是 1px 也就是 1 = 1px)

#### 边距相关

```
p: padding
m: margin
t: top
l: left
r: right
b: bottom
num: [1 ~ 50]

使用实例
<div class="p-10 m-10"></div>
```

#### 文本相关

```
text-[1 ~ 50] 字体大小
text-weight-[100 ~ 900] 字体宽度
line-height-[1 ~ 50] 行高
text-[left, right, center] 文本排列方式(text-align)
text-[primary, black, white] 字体颜色

使用实例
<div class="text-10 text-weight-700 line-height-10 text-center text-black"></div>
```

#### 布局

```
d-flex d-block d-none ...
jc-around jc-center ...
ac-around ac-center ...
ai-center ...
flex-wrap flex-nowrap
flex-grow-[0 ~ 5] flex-shrink-[0 ~ 5]

使用实例
<ul class="d-flex jc-around ai-center flex-wrap">
  <li class="flex-grow-1"></li>
  <li></li>
  <li></li>
</ul>

pos-absolute pos-relative pos-fixed
t-[1 ~ 50] l-[1 ~ 50] ...

使用实例
<div class="pos-relative">
  <div class="pos-absolute t-10 l-10"></div>
</div>
```

### 其他

```
bg-[primary, black, white]

使用实例
<div class="bg-primary"></div>

border-[default, black, white]-[1 ~ 5] 边框 default颜色为灰色可以自己添加变量 大小为1 ~ 5
border-[default, black, white]-[1 ~ 5]--[l, r, b, t] 指定某个方向的边框
border-[default, black, white]-[1 ~ 5]--[solid...] 指定边框类型
border-[default, black, white]-[1 ~ 5]--[l, r, b, t]-[solid...] 指定某个方向边框并指定边框类型

使用实例
<div class="border-default-1"></div>
<div class="border-black-2--b"></div>
<div class="border-black-1--solid"></div>
<div class="border-white-3--b-solid></div>

border-radius-[1 ~ 50]
w[0 ~ 100] 宽度百分比
w-[100 ~ 900] 宽度大小px
h[0 ~ 100]
h-[100 ~ 900]
cursor-[pointer...] 鼠标样式
overflow-[hidden, none...]
bgimg-position-[top, center...] 背景图片定位
bgimg-size-[contain, cover...]
bgimg-[repeat, no-repeat...]
vc-[top, middle, bottom...] vertical-align: top...

手写类名(不通过scss生成)
no-select 用户无法选中
ellipsis 超出省略代替
hover 鼠标悬停样式变化
```
