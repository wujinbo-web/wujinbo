# BootStrap开发梳理
## 尺寸划分 1200px/992px/768px
## container-fluid/container （两容器互相不能嵌套）
1. container  1170px/970px/750px/auto
2. container-fluid 100%
## row/col
1. row 行
2. col-lg-x/col-md-x/col-sm-x/col-xs-x
## 栅格组合模式
- col-lg-4 col-md-6,col-lg-4 col-md-6,col-lg-4 col-md-6
## 常用的样式
1. thumbnail
2. caption
3. btn
4. alert
5. text
6. panel panel-heading panel-body
7. form-group form-control
8. caret dropup/dropdown  箭头  向上向下
## 网格偏移
1. col-[*]-offset-[1-12] 列偏移
2. col-[*]-push/pull-[1-12] 列排序 push往后，pull往前
3. pull-left 左浮动
> offset偏移，当一行有多个元素，偏移的时候超出范围会导致不在一行显示，push/pull不会
## 嵌套之后子集的宽度会根据父集来
## 清楚浮动
- clearfix
## 响应式显示隐藏
1. hidden-[*]  隐藏   
2. visible-[*]-block  显示
## 固定定位 affix
## 字体图标Glyphicons]
- 引入样式
- font-face调整路径
## 预定义样式风格
1. primary 首选样式
2. success 成功
3. info    一般信息
4. warning 警告
5. danger  危险
- btn-primary bg-primary text-primary alert-warning panel-primary
## 按钮类
- 基类btn、a、input
- btn-block   自适应父集宽度
- btn-default 默认无bg带边框，移入有背景
- btn-link    有下划线，像链接
- 按钮默认有大小为bt-md, 设置大小 bt-lg bg-sm bg-xs 
- btn-group 按钮组 按钮之间相互贴合
- btn-group-justifiled  宽度自适应父集 a标签可以，input跟button需要套父集
- btn-group-vertical    横向排列变纵向排列，一般不配合btn-group，不然会产生直角
## 表单类
- 基类form-group form-control
- 调整大小 input-lg input-sm...
- 选中状态 active (选项卡，轮播图之类的)
- 禁用状态 disable 鼠标移入会有禁用手势
## 下拉菜单
1. data-[*] data-toggle="dropdown"  js触发器
2. aria-[*] aria-haspopup="true" 点击是否有内容 aria-expanded="true" aria-labelledby="dropdownMenu1" 目前是否展开  （屏幕阅读器）**一般不同
3. role="menu"  表示的是一个状态   辅助性 **一般不同
4. 下拉菜单必备熟悉  
- 父集 =>class="dropdown"
- button =>class="dropdown-toggle" data-toggle="dropdown"
- ul =>dropdown-menu
5. ul=>dropdown-menu-right  下拉列表靠右显示 





