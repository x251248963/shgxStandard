#JavaScript 编写规范

### 语法

- 声明变量必须加上 var 关键字。

- 常量的形式如: NAMES_LIKE_THIS, 即使用大写字符, 并用下划线分隔。

- 必须加分号。

- 强制转换主要指使用Number、String和Boolean三个构造函数，少用隐式转换。 
参考：http://javascript.ruanyifeng.com/grammar/conversion.html

- **二元运算符两侧必须有一个空格，一元运算符与操作对象之间不允许有空格。**


> var a = !arr.length; 
> 
> a++; 
> 
> a = b + c;


- 使用 ' 优于 "。

- **在 if / else / for / do / while 语句中，即使只有一行，也不得省略块 {...}**。

- 变量、函数在使用前必须先定义。

- 每个 var 只能声明一个变量。

- 变量必须 即用即声明，不得在函数或其它形式的代码块起始位置统一声明所有变量。

- 在 Equality Expression 中使用类型严格的 ===。仅当判断 null 或 undefined 时，允许使用 == null。

- 对于相同变量或表达式的多值条件，用 switch 代替 if。

- 使用对象字面量 {} 创建新 Object。

- 不允许修改和扩展任何原生对象和宿主对象的原型。

> // 以下行为绝对禁止
> 
> String.prototype.trim = function () {
> 
> };

- 使用数组字面量 [] 创建新数组，除非想要创建的是指定长度的数组。

- 遍历数组不使用 for in。 **数组对象可能存在数字以外的属性**

- 尽量避免使用 eval 函数。

- 尽量不要使用 with

- 通过 style 对象设置元素样式时，对于带单位非 0 值的属性，不允许省略单位。

- 优先使用 addEventListener / attachEvent 绑定事件，避免直接在 HTML 属性中或 DOM 的 expando 属性绑定事件处理。使用 addEventListener 时第三个参数使用 false。