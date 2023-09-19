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