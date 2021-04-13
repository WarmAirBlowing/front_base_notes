## 网站的建站流程

![](\img\图片1.png)

## 页面图例

![](\img\未标题-1.jpg)



## 网页的结构

![](img\图片2.png)



## WEB标准

```txt
WEB标准是网页制作的标准，它不是一个标准，它是根据网页的不同组成部分生成的一系列标准。这些标准大部分由W3C起草发布，也有部分标准由ECMA起草发布
```

![](img\图片3.png)

```txt
（1）W3C( World Wide Web Consortium )万维网联盟，创建于1994年是Web技术领域最具权威和影响力的国际中立性技术标准机构；是专门负责网络标准制定的非赢利组织。制定了结构标准和样式标准；
（2）ECMA：欧洲电脑网商联合会（厂商协会），制定了行为标准；
```

## 计算机语言



## HTML

```txt
HTML 指的是超文本标记语言 (Hyper Text Markup Language) www万维网的描述性语言。

XHTML指可扩展超文本标记语言（标识语言）（EXtensible HyperText Markup Language）是一种置标语言，表现方式与超文本标记语言（HTML）类似，不过语法上更加严格。

HTML5指的是HTML的第五次重大修改（第5个版本）
```



### HTML发展

![](\img\图片4.png)



### 编辑器

![](img\1575814575948.png)



### 建立站点

```txt	
规划网站的所有内容和代码
整合资源
```

#### 文件的命名规范

+ 小写英文字母、数字、下划线的组合，
+ 其中不得包含汉字、空格和特殊字符；
+ 必须以英文字母开头。



## HTML开始

### 1：HTML架构

```txt
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">

有三种：  Strict（严格型)、 
             Trasitional（过渡型）、 
             Frameset（框架型）
```

### 2：HTML5基本结构

![](img\1575815336248.png)

### 3:HTML语言

+ HTML语言组成

  + 标签

    + ```txt
      写在尖角号<>里的第一个单词，叫做标记，也叫做标签，也称作元素；
      ```

  + 属性

    + ```
      标记和属性用空格隔开，属性和属性值用等号连接，属性值必须放在双引号内
      一个标记可以有多个属性，属性和属性之间用空格隔开，属性不分先后顺序
      ```

+ **HTML语法**

  + 常规标记(双标记)：
    <标记名称    属性1名="属性1值" 属性2名="属性2值" ………… ></标记名>
  + 空标记（单标记）：<标记名 属性1名="属性1值" />



## 常用标签

### 1 ： 文本标题标签

```txt
文本标题共有6个（h1-h6）
<h1>一级标题</h1>(唯一性,放网站LOGO)
<h2>二级标题</h2>
...
<h6>六级标题</h6> 
```



### 2:字体倾斜&加粗标记

```
文本倾斜:
	<i></i>
	<em></em>
	
文本加粗：
	<b></b>
	<strong></strong>
	
```
### 3 : 段落标记

```
<p></p>
```

p标签的默认样式
        - 换行
                - 有行间距
                - p标签的宽度会跟随浏览器的宽度进行变化

### 4：下划线

```txt
<u></u>
```

### 5 : 换行&水平线

```txt
<br>
<hr>
```

### 6：上标&下标

```txt
<sup></sup>
<sub></sub>
```


### 7 : 字符 （ 小段文本 ）

```txt
<span></span>
```

### 8 : 常用转义字符

```txt
&nbsp;     不换行空格
&gt;       >右尖括号
&lt;       <左尖括号
&copy;     备案中图标版权 ©
&reg;      注册商标 
```

### 8 ：列表

​		（1） 无序列表

```txt	
	<ul>
          <li>列表项内容</li>
          <li>列表项内容</li>
          <li>列表项内容</li>
			   ........   
    </ul>
```

​		（2）有序列表

```txt
	<ol>
          <li>列表项内容</li>
          <li>列表项内容</li>
          <li>列表项内容</li>
			   ........   
    </ol>
```

```txt
type:规定列表中的列表项目的项目符号的类型
语法：<ol       type=“ a"></ol>
1 数字顺序的有序列表（默认值）（1, 2, 3, 4）。
a 字母顺序的有序列表，小写（a, b, c, d）。
A 字母顺序的有序列表，大写（A,B,C,D)
i 罗马数字，小写（i, ii, iii, iv）。
I 罗马数字，大写（i, ii, iii, iv）。

start 属性规定有序列表的开始点。(start的属性值必须是数字)
语法：<ol start="5"></ol>

```

​		（3）自定义列表

```txt	
	<dl>
		<dt></dt>
		<dd></dd>
	</dl>
```

### 9 : 超链接

```txt
<a></a>
	属性：
		href = 'url'
		target = "_black  /  _self";
		title = '文本提示'
	 默认样式
            - 有字体颜色
            - 下线划
            - 有默认的手型 引导用户去点击跳转
		
	拓展1：
		rel = 'nofollow';  告诉搜索引擎“不要追踪此网页上的链接”或”不要追踪此特定链接”；
		- nofollow的几个作用
            ① 可以防止页面中不可信的内容
            ② 付费信息链接 谷歌浏览器推荐使用的属性
            ③ 引导爬虫去爬取页面中的有效信息:避免爬取一些无效的信息，影响爬虫效率
        - nofollow的使用方式
            - 使用a标签     <a rel="nofollow"> 表示当前的a 标签不需要被跟踪
           	- 使用meta标签  <meta content="nofollow"> 推荐使用 当前页面上的所有超链接都不需要被跟踪
		
		例：<a href="signin.php" rel="nofollow">用户注册</a>
		
		以下是经常用到nofollow的几种情况：
	       1、不可信赖的内容
           2、付费链接
           3、按优先级别进行抓取
           
		
	拓展2：	
		 <base />   标签为页面上的所有链接规定默认地址或默认目标。
		 
		 例：<base target="_blank" />
		 
		 注：<base> 标签必须位于 head 元素内部。
	拓展3：
		当检测到一个压缩文件时，就会自动下载
		 <a href="demo.rar">点击下载</a>
		 
	 超链接标签点击跳转的页面没有固定的地址吗，那么href的跳转地址需要如何设置？
            - ###
            - javascript:; 造成浏览器阻塞
```

### 10 : 图片

```
<img>
	属性：
		src = 'url';
		alt = ' 标签 实例 带有指定替代文本的图像'  
        title = '文本提示'
		width = ''
		height = ''
		border = ''
```

##### 图片 title 和 alt区别：

```txt
	alt:
        1、alt属性是考虑到不支持图像显示或者图像显示被关闭的浏览器的用户，以及视觉障碍的用户和使用屏幕阅读器的用户。当图片不显示的时候，图片的替换文字。
        2、alt属性值得长度必须少于100个英文字符
        3、alt属性是img标签的必须属性，如果没有特别意义的图片，可以写alt=""
        4、alt属性是搜索引擎判断图片与文字是否相关的重要依据，alt属性添加到img主要的目的才是为了SEO
        
    title:
    	1、title属性并不是必须的。
        2、title属性规定元素的额外信息，有视觉效果，当鼠标放到文字或是图片上时有文字显示。
        3、title属性并不作为搜索引擎抓取图片的参考，更多倾向于用户体验的考虑。
```

### 11 : 相对路径

```txt
（同级）
	1)当当前文件与目标文件在同一目录下，直接书写目标文件的文件名+扩展名；
（上级找下级）
	2)当当前文件与目标文件所处的文件夹在同一目录下，写法如下：
	文件夹名/目标文件全称+扩展名；
（下级找上级）
	3)当当前文件所处的文件夹和目标文件在同一目录下，写法如下：
	../目标文件文件名+扩展名；
	
	
	
	/   :  从根目录出发
	./  :  从当前位置出发   和不写的效果是一样的
	../ :  返回上一层
```

### 12 ： DIV

### 13 : HTML注释

```html
<!-- 注释 -->
```



## 表格

![](img\22222.png)

#### 1 : 表格基本结构

```html
<table>
	<tr>
		<td></td>
		<td></td>
	</tr>
</table>

<!-- 
	table 为表格
	tr  行
	td  列（每一个单元格）
-->
```

#### 2 ： 数据行分组

```html
<thead></thead>  表头  （一个表格里只能有一个）
<tbody></tbody>  表体
<tfoot></tfoot>  表尾  （一个表格里只能有一个）
```

#### 3 ： 数据列分组

```html
<colgroup span="value"></colgroup>
<!--span属性为把几列分为一组-->
```

#### 3 ： 列标题

```html
<th></th>
```

#### 4 : 表格标题

```html
<caption></caption>
```

#### 5：表格的html属性

```txt
1）width="表格的宽度"
2）height="表格的高度"
3）border="表格的边框"
4）bordercolor="边框色"
5）cellspacing="单元格与单元格之间的间距"
6）cellpadding=“单元格与内容之间的距离"
7）align="表格水平对齐方式"
   取值：left、right、center、
   valign=“垂直对齐” top\bottom\middle
8）合并单元格属性：(td)
  合并列： colspan=“所要合并的单元格的列数"
  合并行： rowspan=“所要合并单元格的行数”
9） rules="rows/cols/all/none/groups"    添加分隔线
	说明：
		rows:位于行之间的线条
		cols:位于列之间的线条
		all：位于行和列之间的线条
		none:没有线条
		groups:位于行组和列组之间的线条
```



## 表单

#### 1 ： 表单标签

```html
<form></form>
	属性 ： 
		action = '接口地址'
		method = 'get / post'
		name = '表单名称'
```

#### 2 ： 表单控件

```txt
<input>
	属性：
		type = '控件类型'
		name：属性标识表单域的名称；
		Value：属性定义表单域的默认值，其他属性根据type的不同而有所变化。
		maxlength：控制最多输入的字符数，
		Size：控制框的宽度（以字符为单位）
```

```txt
1）文本框
	<input type="text" value="默认值"/>
2)密码框
	<input type="password" />
3)提交按钮
	<input type="submit" value="按钮内容" />
4)重置按钮
	<input type="reset" value="按钮内容" />
5)空按钮
	<input type="button" value="按钮内容" />
6）单选按钮组
    <input type=“radio” name=“ral” />男
    <input type=“radio” name=“ral”
    checked=“checked”/>(默认选中)女
7）复选框组
    <input type="checkbox" name="" />
    <input type="checkbox" name="" disabled="disabled" />
     *  disabled="disabled" (禁用)
     *  checked="checked"   (默认选中)
8）下拉列表（菜单）：
	<select >
   		<option>下拉选项1</option>
   		<option>下拉选项2</option>
   		…………
	</select>
	表示下拉列表，name属性不是必须的
	默认选择项用selected属性；
9）表单域多行文本定义：
	语法:	<textarea name=""  cols=""  rows="" ></textarea>
	多行文本。rows属性和cols属性用来设置文本输入窗口的高度和宽度，单位是字符。
	阻止浏览器对窗口的拖动设置:{resize:none;}（css属性）
10)上传文件：
	语法：<input type="file">
11）隐藏表单，一般用作数据存储
文件域：<input type="hidden" value="订单编号" /> 这是隐藏表单,一般用来传递参数,而又不想显示在客户端。
 
```

#### 3 : 表单标签

```txt
1）表单字段集
语法：<fieldset></fieldset>

说明：相当于一个方框，在字段集中可以包含文本和其他元素。该元素用于对表单中的元素进行分组并在文档中区别标出文本。fieldset元素可以嵌套，在其内部可以在设置多个fieldset对象。disabled定义空间禁制可用；

2）字段级标题：
语法：<legend align="left/center/right/justify"></legend>
说明：legend元素可以在fieldset对象绘制的方框内插入一个标题。legend元素必须是fieldset内的第一个元素。
3)提示信息标签：
语法：<label for="绑定控件id名"></label>

说明：label元素用来定义标签，为页面上的其他元素指定提示信息。要将label元素绑定到其他的控件上，可以将label元素的for属性设置为与该控件的id属性值相同。
```







## 拓展：post/get

+ (1). 从功能上讲，GET一般用来从服务器上获取资源，POST一般用来更新服务器上的资源；

+ (2). 从REST服务角度上说，GET是幂等的，即读取同一个资源，总是得到相同的数据，而POST不是幂等的，因为每次请求对资源的改变并不是相同的；进一步地，GET不会改变服务器上的资源，而POST会对服务器资源进行改变；

+ (3). 从请求参数形式上看，GET请求的数据会附在URL之后，即将请求数据放置在HTTP报文的 请求头 中，以?分割URL和传输数据，参数之间以&相连。特别地，如果数据是英文字母/数字，原样发送；否则，会将其编码为 application/x-www-form-urlencoded MIME 字符串(如果是空格，转换为+，如果是中文/其他字符，则直接把字符串用BASE64加密，得出如：%E4%BD%A0%E5%A5%BD，其中％XX中的XX为该符号以16进制表示的ASCII)；而POST请求会把提交的数据则放置在是HTTP请求报文的 请求体 中。

+ (4). 就安全性而言，POST的安全性要比GET的安全性高，因为GET请求提交的数据将明文出现在URL上，而且POST请求参数则被包装到请求体中，相对更安全。

+ (5). 从请求的大小看，GET请求的长度受限于浏览器或服务器对URL长度的限制，允许发送的数据量比较小，而POST请求则是没有大小限制的。
  