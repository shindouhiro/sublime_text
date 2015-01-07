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
```


