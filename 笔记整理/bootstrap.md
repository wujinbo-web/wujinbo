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
- 基类form-group分组  form-control 输入框  placeholder="ahdd" 默认值
- 调整大小 input-lg input-sm...
- 选中状态 active (选项卡，轮播图之类的)
- 禁用状态 disabled 鼠标移入会有禁用手势
- input-group-addon
## 下拉菜单
1. data-[*] data-toggle="dropdown"  js触发器
2. aria-[*] aria-haspopup="true" 点击是否有内容 aria-expanded="true" aria-labelledby="dropdownMenu1" 目前是否展开  （屏幕阅读器）**一般不同
3. role="menu"  表示的是一个状态   辅助性 **一般不同
4. 下拉菜单必备熟悉  
- 父集 =>class="dropdown"
- button =>class="dropdown-toggle" data-toggle="dropdown"
- ul =>dropdown-menu
5. ul=>dropdown-menu-right  下拉列表靠右显示 
6. dropdown-header  列表头
7. dropdown-divider 列表分割线
8. li =>text-center
## 如何判断是否为PC端
- if(window.navigator.userAgent.toLowerCase().indexOf('mobile')==-1)
## data-target=".dropdown" 控制另外的菜单
## 头部
1. nav
2. nav-tabs
3. nav-justifiled        按钮自适应父集宽   废弃
4. nav-tabs-justifiled    线自适应按钮宽     废弃
5. nav-pills		 有背景的样式
6. nav-stacked		 有背景竖状菜单    nav-pill + nav-stacked  配合    nav-tabs有bug
## 内容
1. ul  =>  tab-content
2. li  =>  tab-pane    
3. a   =>  data-toggle="tab"
4. 内容切换加ID ，用href="#a" 进行锚点切换
5. fade in 淡入淡出
6. 鼠标移入
$('#myTab a').mouseover(function(){
      $(this).tab('show');
    });
## 导航
1. nav  =>  navbar navbar-default 白色调  navbar-inverse 黑色调
2. ul   =>  nav navbar-nav    navbar-rigth 在右侧显示
3. navbar-static-top  两边的圆角变直角
4. navbar-fixed-top/navbar-fixed-bottom    固定定位
5. 固定定位遮挡问题  给Body加margin-top:50px;
6. div 父= > navbar-header    子a  =>  navbar-brand 加logo
7. navbar-btn 导航加按钮  navbar-link 导航加链接  navbar-left navbar-text文字垂直居中 navbar-form
## 下拉导航条
1. button => navbar-toggle 移动端导航按钮   data-toggle="collapse"  data-target="#...."
2. span   => icon-bar      横线
3. 给ul加div父集  =>  collapse navbar-collapse    加ID对应data-target
## 滚动监听
1. Body =>  relative  data-spy="scroll" 滚动监听 data-target="#myNavrbar" 监听对象 data-offset="60" 对象距离顶部的距离
2. nav =>  id="myNavbar"


## 媒介特征
1. max-width
2. min-width
## 媒体关键词
1. not
2. and
3. only

- @media all and (min-width:960){} 媒询