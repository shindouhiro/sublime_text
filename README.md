sublime_text
============

#快捷键与插件介绍
##快捷
(sublime.html)
<table>
    <tr>
			<td>Ctrl+L</td>
			<td>选择整行(按住-继续选择下行)</td>
		</tr>
		<tr>
			<td>Ctrl+KK</td>
			<td>从光标处删除至行尾</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+K</td>
			<td>删除整行</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+D</td>
			<td>复制光标所在整行，插入在该行之前</td>
		</tr>
		<tr>
			<td>Ctrl+J</td>
			<td>合并行(已选择需要合并的多行时)</td>
		</tr>
		<tr>
			<td>Ctrl+KU</td>
			<td>改为大写</td>
		</tr>
		<tr>
			<td>Ctrl+KL</td>
			<td>改为小写</td>
		</tr>
		<tr>
			<td>Ctrl+D</td>
			<td>选词(按住-继续选择下个相同的字符串)</td>
		</tr>
		<tr>
			<td>Ctrl+M</td>
			<td>光标移动至括号内开始或结束的位置</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+M</td>
			<td>选择括号内的内容(按住-继续选择父括号)</td>
		</tr>
		<tr>
			<td>Ctrl+/</td>
			<td>注释整行(如已选择内容，同“Ctrl+Shift+/”效果)</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+/</td>
			<td>注释已选择内容</td>
		</tr>
		<tr>
			<td>Ctrl+Space</td>
			<td>自动完成(win与系统快捷键冲突，需修改)</td>
		</tr>
		<tr>
			<td>Ctrl+Z</td>
			<td>撤销</td>
		</tr>
		<tr>
			<td>Ctrl+Y</td>
			<td>恢复撤销</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+V</td>
			<td>粘贴并自动缩进(其它兄弟写的，实测win系统自动缩进无效)</td>
		</tr>
		<tr>
			<td>Ctrl+M</td>
			<td>光标跳至对应的括号</td>
		</tr>
		<tr>
			<td>Alt+.</td>
			<td>闭合当前标签</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+A</td>
			<td>选择光标位置父标签对儿</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+[</td>
			<td>折叠代码</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+]</td>
			<td>展开代码</td>
		</tr>
		<tr>
			<td>Ctrl+KT</td>
			<td>折叠属性</td>
		</tr>
		<tr>
			<td>Ctrl+K0</td>
			<td>展开所有</td>
		</tr>
		<tr>
			<td>Ctrl+U</td>
			<td>软撤销</td>
		</tr>
		<tr>
			<td>Ctrl+T</td>
			<td>词互换</td>
		</tr>
		<tr>
			<td>Ctrl+Enter</td>
			<td>插入行后</td>
		</tr>
		<tr>
			<td>Ctrl+Shift Enter</td>
			<td>插入行前</td>
		</tr>
		<tr>
			<td>Ctrl+K Backspace</td>
			<td>从光标处删除至行首</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+UP</td>
			<td>与上行互换</td>
		</tr>
		<tr>
			<td>Ctrl+Shift+DOWN</td>
			<td>与下行互换</td>
		</tr>
		<tr>
			<td>Shift+Tab</td>
			<td>去除缩进</td>
		</tr>
		<tr>
			<td>Tab</td>
			<td>缩进</td>
		</tr>
		<tr>
			<td>F9</td>
			<td>行排序(按a-z)</td>
		</tr>
</table>
##插件
Emmet html/CSS(使用方法emmet.html)  
快速编辑（原名Zen Coding）  
其他的看自己需求百度(几乎无所不有，这就是sublime强大的原因之一)


#Emmet快捷键
1.简写Div
```php
type this:
div.container

or this:
.container

get this:
<div class="container"></div>
```

2.含糊标签名称
```php
type this:
.wrap>ul.list>.sites

get this:
<div class="wrap">
	<ul class="list">
		<li class="sites"></li>
	</ul>
</div>
```

3.带有DOM导航的链式缩写
* > 子节点：在DOM树下一层添加创建一个元素
* + 同级别：在DOM树同一层添加创建一个元素
* ^ 向上层：向上一层添加创建创建一个元素。

```php
type this:
.outer>.inner>h1+p

get this:
<div class="outer">
	<div class="inner">
		<h1></h1>
		<p></p>
	</div>
</div>


type this:
.warp>p>a^p

get this:
<div class="warp">
	<p><a href=""></a></p>
	<p></p>
</div


type this:
.wrap>p>em>a^^p

get this:
<div class="wrap">
	<p><em><a href=""></a></em></p>
	<p></p>
</div>

type this:
(.one>h1)+(.two>h1)

get this:
<div class="one">
	<h1></h1>
</div>
<div class="two">
	<h1></h1>
</div>
```

4. 使用分组来简化你的代码结构
```php
type this:
(section>.wrap>h1>p>a)+(section>.wrap>p+p)

get this:
<section>
	<div class="wrap">
		<h1>
			<p><a href=""></a></p>
		</h1>
	</div>
</section>
<section>
	<div class="wrap">
		<p></p>
		<p></p>
	</div>
</section>
```

5. 插入文本和属性
```php
type this:
h1{Heading}+p{lorem ipsum}

get this:
<h1>Heading</h1>
<p>lorem ipsum</p>

type this:
a[href="http://www.apple.com"]{Apple}

get this:
<a href="http://www.apple.com">Apple</a>
```

6. 添加多个class到一个元素
```php
type this:
.one.two.three

get this:
<div class="one two three"></div>
```

7.  重复添加
```php
type this:
ul>li*3

get this:
<ul>
	<li></li>
	<li></li>
	<li></li>
</ul>

type this:
(section>.wrap)*2

get this:
<section>
	<div class="wrap"></div>
</section>
<section>
	<div class="wrap"></div>
</section>
```

8. 自动列表记数
```php

type this:
ul>li.item${item $$}*3

get this:
<ul>
	<li class="item1">item 01</li>
	<li class="item2">item 02</li>
	<li class="item3">item 03</li>
</ul>
```


