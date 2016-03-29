#CSS 编写规范

常用的css命名规则：
	* 头：header
	* 内容：content/container
	* 尾：footer
	* 导航：nav
	* 侧栏：sidebar
	* 栏目：column
	* 页面外围控制整体布局宽度：wrapper
	* 左右中：left right center
	* 登录条：loginbar
	* 标志：logo
	* 广告：banner
	* 页面主体：main
	* 热点：hot
	* 新闻：news
	* 下载：download
	* 子导航：subnav
	* 菜单：menu
	* 子菜单：submenu
	* 搜索：search
	* 友情链接：friendlink
	* 页脚：footer
	* 版权：copyright
	* 滚动：scroll
	* 内容：content
	* 标签页：tab
	* 文章列表：list
	* 提示信息：msg
	* 小技巧：tips
	* 栏目标题：title
	* 加入：joinus
	* 指南：guild
	* 服务：service
	* 注册：regsiter
	* 状态：status
	* 投票：vote
	* 合作伙伴：partner

id的命名：(1)页面结构

	* 容器: container
	* 页头：header
	* 内容：content/container
	* 页面主体：main
	* 页尾：footer
	* 导航：nav
	* 侧栏：sidebar
	* 栏目：column
	* 页面外围控制整体布局宽度：wrapper
	* 左右中：left right center

(2)导航

	* 导航：nav
	* 主导航：mainbav
	* 子导航：subnav
	* 顶导航：topnav
	* 边导航：sidebar
	* 左导航：leftsidebar
	* 右导航：rightsidebar
	* 菜单：menu
	* 子菜单：submenu
	* 标题: title
	* 摘要: summary

(3)功能

	* 标志：logo
	* 广告：banner
	* 登陆：login
	* 登录条：loginbar
	* 注册：regsiter
	* 搜索：search
	* 功能区：shop
	* 标题：title
	* 加入：joinus
	* 状态：status
	* 按钮：btn
	* 滚动：scroll
	* 标签页：tab
	* 文章列表：list
	* 提示信息：msg
	* 当前的: current
	* 小技巧：tips
	* 图标: icon
	* 注释：note
	* 指南：guild
	* 服务：service
	* 热点：hot
	* 新闻：news
	* 下载：download
	* 投票：vote
	* 合作伙伴：partner
	* 友情链接：link
	* 版权：copyright

class的命名：(1)颜色:使用颜色的名称或者16进制代码,如

	* .red { color: red; }
	* .f60 { color: #f60; }
	* .ff8600 { color: #ff8600; }

（2）字体大小,直接使用”font+字体大小”作为名称,如

	* .font12px { font-size: 12px; }
	* .font9pt {font-size: 9pt; }

(3)对齐样式,使用对齐目标的英文名称,如

	* .left { float:left; }
	* .bottom { float:bottom; }

(4)标题栏样式,使用”类别+功能”的方式命名,如

	* .barnews { }
	* .barproduct { }

注意事项::

	1. 一律小写;
	2. 尽量用英文;
	3. 不加中杠和下划线;
	4. 尽量不缩写，除非一看就明白的单词.




### 语法

- **不要使用 @import**

- 用两个空格来代替制表符（tab） -- 这是唯一能保证在所有环境下获得一致展现的方法。

- 为选择器分组时，将单独的选择器单独放在一行。

- 为了代码的易读性，在每个声明块的左花括号前添加一个空格。

- 声明块的右花括号应当单独成行。

- 每条声明语句的 : 后应该插入一个空格。

- 为了获得更准确的错误报告，每条声明都应该独占一行。

- 所有声明语句都应当以分号结尾。最后一条声明语句后面的分号是可选的，但是，如果省略这个分号，你的代码可能更易出错。

- 对于以逗号分隔的属性值，每个逗号后面都应该插入一个空格（例如，box-shadow）。

- 不要在 rgb()、rgba()、hsl()、hsla() 或 rect() 值的内部的逗号后面插入空格。这样利于从多个属性值（既加逗号也加空格）中区分多个颜色值（只加逗号，不加空格）。

- 对于属性值或颜色参数，省略小于 1 的小数前面的 0 （例如，.5 代替 0.5；-.5px 代替 -0.5px）。

- 十六进制值应该全部小写，例如，#fff。在扫描文档时，小写字符易于分辨，因为他们的形式更易于区分。

- 尽量使用简写形式的十六进制值，例如，用 #fff 代替 #ffffff。

- 为选择器中的属性添加双引号，例如，input[type="text"]。只有在某些情况下是可选的，但是，为了代码的一致性，建议都加上双引号。

- 避免为 0 值指定单位，例如，用 margin: 0; 代替 margin: 0px;。

注释的写法：
/* Footer */
内容区
/* End Footer */