1. container 容器
2. container-fluid  宽度100%

#### 栅格系统 栅格系统默认占据12列分

class名

1. row 表示一行
2. col-**xl**-x  **x** 表示要站多少列分 xl表示最大宽度 sm、md、lg、xl 最大宽度从小到大 如果该参数没有写则不会出现单独站一行的情况 col-auto 表示该元素本身多大就多大 xl表示到什么宽度会恢复默认
3. 等宽概念：单写col 不会自动换行需手动添加 w-100 表示换行 
4. 混合布局 col-sm col-md col-lg col-xl
5. 元素对齐方式 行：y轴： align-items-[start、end、center] 设置水平居中 align-self-[start、end、center]   设置单个元素  x轴：justify-content

6.no-gutter 加在row上清楚内边距

7.order 子元素排列 默认是1 越大排越后 order-first 排第一位

8.offset-x   x表示偏移几个列份

9.ml-auto  mr-auto 表示强制向左或右隔开

10.列嵌套 

### 禁用响应式?

1. 把meta先删除

2. 给盒子设置宽度

   ### 设置响应式分界点

   在Bootstrap的源Sass文件中，为了实现布局、网格系统以及组件，首先使用下面的媒体查询范围(可 以理解为将不同宽度的网页进行拆分并分别载入CSS样式处理构建）：

### 排版

1. 标题 

   副标题`<small class="text-muted">副标题</small>` 写在标题里面

   display-x  表示让标题更大

2. lead 表示重要文本内容标签

3. mark 高亮标签

4. ins 下划线标签

5. del 删除线标签

6. strong 粗体字体

7. abbr 下划线虚线 标签 加title

8. block quote标签 来源备注与引用 需加block quote类 常用与尾部识别；footer标签 需加blockquote-footer类 cite标签

9. ul and li；.list-unstyled 去小圆点加在ul，不会影响到嵌套的；.list-inline 默认显示行，,list-inline-item 表示按列显示 ul写list-line li 写list-inline-item

10. .text-truncate 文本溢出以省略号结束

11. var标签  提示var变量

12. kbd 标签 提示这是用键盘输入的指令

13. samp标签表示这个是示例

#### 图片and图片框

1. .img-fluid 充满
2. w-100 撑满
3. img-thumbnail 加个圆角边框
4. 图片对齐方式 浮动布局float-left；给父元素加.clearfix .rounded圆角效果；d-xxx xxx表示转换成什么类型的盒子；图片居中两种方法1加.mx-auto 需转换元素类型,2.给父盒子加.text-center
5. H5新picture标签 里面写source标签 media="(min-widt h: 800px)" 属性表示不同屏幕显示不同图片
6. 图文框

### 表格

1. 在table 加table类即可生成
2. table-dark在table加则全部产生颜色反转对比 thead-light | thead-dark表头也可以
3. table-striped 定义tbody隔行换色 条纹状表格可配合table-fark使用
4. table-bordred 产生表格边框 table-borderless 无边框
5. table-sm 使表格更紧凑
6. 语义化 table-active.... 使行或列或单格换色
7. bg-info .... 改变背景颜色
8. caption标签表示该表格的标题

### 边框

1. border-top|四个方向指定
2. border-top-0 删除指定边框
3. border-xxx 边框颜色
4. rounded-方向
5. rounded-circle 圆型边框
6. rounded-pill 两边圆型
7. rounded-0 清除圆形
8. clearfix 清除浮动

### 颜色display

1. text-xxx 
2. d-{sm|md|lg|xl}-inline|block|inline|block|flex|table-row|table-cell
3. d-{sm|md|lg|xl}-none 隐藏元素 
4. d-print-block  打印时显示

### 文本对齐 默认左对齐

1. text-[断点]-center|left|right|justify justify结尾不会留空白
2. text-truncate 溢出省略号处理 该元素必须是块元素
3. text-nowrap  强制一行输出
4. text-lowercase 文本全部小写
5. text-uppercase 文本全部大写
6. text-capitalize 首字母大写
7. font- weight-bold|normal|light|italic 文本粗细
8. text-monospace 等宽字体
9. align-top|bottom|middle|baseline   表格也可使用
10. h|w-25|50|75|100 设置宽高百分比
11. mh-100 mw-100 最大宽度

### 间隔和阴影

1. m=margin p=padding t|b|l|r|x|y x=l&r y = t|b
2. shadow-none | shadow{lg|sm} 阴影大小

### 定位

1. postion-relative|absolute 
2. fiexd-top|bottom
3. sticky-top|bottom
4. visibility | invisibility 显示元素
5. close 用于按钮或a标签 

### 嵌入

1. iframe
2. text-hide 文字隐藏 可替换为背景图片 
3. sr-only 隐藏
4. sr-only-focusable 当获得焦点并按下tab则会显示 

### flex 都可加断点

1. 子元素：flex-fill == flex：1等分 自项等
2. 子元素：flex-grow-0|1
3. flex-shrink-0 缩小 1为本身宽度
4. 自浮动：水平：ml-auto mr-auto 垂直：mt-auto mb-auto

### 警告框 可加其他元素

1. alert类 alert-xxx [颜色]
2. alert-heading 警告框标题
3. alert-link a标签
4. 按钮解除警告 alert-dismissible 按钮样式  按钮加data-dismiss='alert' 要想移除有效果则加 fade show类在alert盒子

### 徽章 badge

1. badge 可用于a链接标题按钮
2. badge-pill

### 面包屑导航 

1. breadcrumb 主盒子
2. breadcrumb-item  子元素 active表示当前页面显示

### 按钮

1. btn btn-颜色 a链接也可使用
2. btn-outline-颜色  轮廓按钮 边框有颜色
3. btn-lg|sm|block  按钮尺寸
4. disabled 禁用状态
5. 切换状态 加自定义属性 data-toggle='button' = 切换active 
6. btn-group 管理包含在btn-group里面的btn元素 在btn—group里input按钮加data-toggle='buttons' 进行切换 bootstrap4提供了全新的复选框 btn-group-toggle js里切换 xxx.button('toggle')
7. btn-toolbar 父盒子 管理多个按钮组
8. btn-group-vertical 垂直排列 

### 下拉菜单 dropdown

1. dropdown 定义块级元素
2. dropdown-menu 定义菜单
3. dropdown-item 菜单选项
4. dropdown-toggle  三角型
5. 采用分裂式显示的话则需要设置btn-group
6. 自定义属性 data-toggle="dropdown"
7. dropup|dropleft|dropright 定义在父盒子 菜单出现在哪个方向上
8. B3下拉只能是a标签 B4能是任意标签
9. active&disable 高亮与禁用
10. drop-menu-right 对齐方式 如果想使用响应式对齐则需要禁用动态定位 data-display='static'
11. 分割线使用 div.dropdown-divider
12. data-offset=''  下拉菜单偏移
13. data-reference=‘parent’ 以谁对齐

### 输入框

1. 输入组 input-group
2. 在input前面 input—group-prepend
3. 在input后面 Input-group-append
4. 文字input-group-text
5. 可加按钮、表单、其他元素.....

### 表单

1. form-group
2. form-control-[ls|sm] 宽度变为100 % 文本控件统一使用 如text、text area 、select
3. 文件上传则需要 form—control-file
4. form-control-range 选中范围 input为range
5. 标签定义 readonly 只读
6. 提示文本 标签 small.form-text.text-muted
7. form-check-label 与复选框对齐 form-check 盒子
8.  form-check 用来格式化单选和复选包住他们
9. form-check-input 单选和复选
10. form-chec-inline 使form-check里面的单选和复选水平排列
11. 可使用栅格布局 form-group可一同连col写 
12. form-row 相比于 row 列间隔更窄 
13. 使用栅格布局form时label会对不齐使用col-form-label 即可对齐

<div class="form-group row">
							<label for="" class="col-2 col-form-label">邮箱</label>
							<input type="text" class="form-control col-10">		 

```html
			</div>
```

14.form-inline 使表单元素都一行显示

15.disabled 禁用单个表单 fieldset标签里使用disabled 整个表单都禁用

16.form-control-plaintext 移除表单样式

17.表单验证：require必填  给form标签添加needs-validation类

18.自定义表单 custom-checkbox custom-control-input  ？？？

19.ios风格开关 

### 轮播图

1. carousel  加自定义属性data-side='carousel' 开始滚动 data-interval=‘毫秒’ data-pause='pause|false' 鼠标移入是否停止 
2. carousel-inner
3. carousel-item
4. carousel-wrap  到最后一张是否重新播放
5. carousel-control-prev|carousel-control-next  上一张或下一张  `<a class="carousel-control-prev text-primary" data-slide='prev' href="#myCarousel"><span class="carousel-control-prev-icon"></span></a>`
6. 状态显示 
7. 字幕提示 在carousel-item里 carousel-caption d-none d-sm-block 
8. 交替变化 carousel-fade|slide
9. 延迟 carousel-interval可加在carousel-item里重新定义滑动时间

### 广告大块屏幕 列表

<div class="jumbotron">
			  <h1 class="display-3">Hello, world!</h1>
			  <p class="lead">This is a simple hero unit, a simple jumbotron-style
			component for calling extra attention to featured content or information.</p>
			  <hr class="my-4">
			  <p>It uses utility classes for typography and spacing to space content out
			within the larger container.</p>
			  <p class="lead">
			  <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
			  </p>
			  </div>

### 列表组

1. list-group
2. list-group-item  可被active也可disabled 按钮a标签都可用
3. list-group-item-颜色
4. list-group-item-action 加经过样式
5. list-group-flush 去除圆角边框

自定义布局

### 媒体对象

1. media 定义media盒子
2. media-body 里面加标题和内容 

可用于写新闻列表   list-unstyled

`<div class='media'><div class='media-body'>img title content</div></div>`

### 弹出消息框 toast

1. 定义toast盒子 data-autohide='true|false 是否自动隐藏 data-delay='隐藏间隔' data-animation='true|false' 隐藏是否淡出淡入 默认是隐藏  
2. toast-header 标题
3. toast-body 内容主体
4. JavaScript 

### 提示冒泡 tooltip

1. 用于title提示 data-toggle='tooptip'
2. 还需js启动 $([data-toggle='tooptip']).tooltip()
3. data-html='true|false'  自定义提示可加html标签
4. data-animation|delay=[number|{'hide':time,'show':m}]|trigger='click|focus|hover|dclick'|offset=''|placement='方向'|html
5. javascript事件  xxx.tooltip('show|hide|toggle')

### POP提示 popover

1. 用于a标签或者按钮或其他元素点击时出现提示信息 data-toggle='popover' 
2. data-animation|delay|trigger|placement|offset|html
3. data-content='' 提示文本信息 标题是title 内容则是data-content
4. javascript事件跟提示冒泡一样

### 弹出模态框 modal

默认隐藏

1. modal 父盒子
2. modal-dialog 
3. modal-content 内容区域 modal-header   modal-title modal-body  modal-footer 
4. tabindex='-1' 属性表示按esc可以退出modal框
5. data-backdrop='true|false' 背景是否覆盖阴影
6. modal-dialog-centered 居中 
7. data-delay|animation

### 导航-滑动门

1. nav
2. nav-item
3. nav-link
4. 水平对齐使用justify-content-center
5. 垂直排列  flex-column
6. nav-tabs 滑动门 navpills
7. nav-fill nav-item 不是每个都是一样
8. nav-justifed 相比于nav-fill 平均分配
9. tab-content 嵌套tab-pane 配合nav-tabs或nav-pills 使用 data-toggle='tab' a链接指向nav-pane的id或data-target=‘#id’

### 导航栏

1. navbar
2. navbar-brand  公司名或logo
3. nav-expand-{断点} 什么时候
4. navbar-nav 
5. collapse navbar-collapse 导航栏折叠面板 
6. 当缩小到断点时会出现按钮 navbar-toggler 按下折叠面板会出现

### 卡片  card

1. card
2. card-body > card-title > card-subtitle副标题>card-header 页眉 card-footer页脚 
3. card-text  card-link
4. card-img-top|bottom   
5. card-img-overlay 替换掉card-body 背景图片
6. 可加列表组 
7. 三种排列方式 card-group 水平没有间隔 card-deck 卡牌 垂直没有间隔 card-columns

### 折叠面板 Collapse

1. 按钮 data-toggle=‘collapse’ data-target=''
2. class='collapse' 

### 分页 进度条

本身是flex 采用flex居中

1. pagination  page-item page-link
2. progress

### 滚动监听

1. 

### 旋转特效

1. spinner-border-[sm]加颜色用text-xxx
2.  spinner-grow  渐变
3. 可加在按钮里面

