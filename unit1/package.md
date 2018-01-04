### 简史

就职于 Netscape 公司的布兰登 艾奇（Brendan Eich），开始着手为计划1995年2月发布的Netscape Navigator 2 开发一种
名为LiveScript 的脚本语言——该语言将同时在浏览器和服务器中使用（在服务器上的名字叫 LiveWire）

微软在其Internet Explorer 3 中加入名为JScript的javascript实现。

1997年，以javascript1.1 为蓝本的建议提交给了欧洲计算机制造协会（ECMA）

### 实现

javascript 由下列三个不同的部分组成

核心：ECMAScript
文档对象模型：DOM
浏览器对象模型：BOM

##### ECMAScript 版本

1. ECMAScript 第一版与Netscape 的javascript1.1 相同，做了一些小改动：支持Unicode，
2. ECMAScript 第二版主要是编辑加工，
3. ECMAScript 第三版是对该标准第一次真正的修改，修改内容涉及字符串处理，错误定义和数值输出。
该版新增了正则表达式，新控制语句，try-catch异常处理。
4. ECMAScript 第四版对语言进行了一次全面的检核修订。不仅包含强类型变量，新语句和新数据结构
真正的类和经典继承，还定义了与数据交互的新方式。第四版给这门语言带来的跨越太大了。在发布前被放弃。
5. ECMAScript 3.1 即 ECMAScript 第五版，添加了原生JSON对象（用于解析和序列化JSON数据），继承的方法
和高级属性定义，还包含一种严格模式。

##### DOM
    文档对象模型（DOM）是针对XML但经过扩展用于HTML的应用程序编程接口（API）。DOM把整个页面映射为一个多层节点结构。

1. 负责制定Web通信标准的W3C开始着手规划DOM
2. DOM 级别。
   1. DOM1级（DOM Level 1）于1998年10月成功W3C的推荐标准。DOM1由两个模块组成：DOM核心（DOM Core）和 DOM HTML.
   2. DOM2级（DOM Level 2）在原来的DOM的基础上有扩充了（DHTML一直都支持的）鼠标和用户界面事件、范围、遍历（迭代DOM文档的方法）
   等细分模块，而且通过对象接口增加了对CSS的支持。
   DOM2级引入了下列模块
        1. DOM视图（DOM Views）：定义了跟踪不同文档视图的接口。
        2. DOM事件（DOM Events）：定义了事件和事件处理的接口。
        3. DOM样式（DOM Style）：定义了基于CSS为元素应用样式的接口。
        4. DOM遍历和范围（DOM Traversal and Range）：定义了遍历和操作文档树的接口。
   3. DOM3级（DOM Level 3）则进一步扩展了DOM，引入了统一方式加载和保存文档方法——在DOM加载和保存（DOM Load and Save）模块中定义
   新增了验证文档的方法——在DOM 验证（DOM Validation）模块中定义。DOM3级也对DOM核心进行了扩展，涉及XML Infoset，XPath和 XML Base.
3. 其他DOM标准
    1. SVG(可伸缩矢量图)1.0
    2. MathML(数学标记语言)1.0
    3. SMIL(同步多媒体集成语言)

##### BOM
    访问和操作浏览器窗口的浏览器对象模型（BOM）.开发人员使用BOM可以控制浏览器显示的页面以为的部分。
    而BOM真正与众不同的地方（也是经常会导致问题的地方），还是它作为javascript实现的一部分但却没有相关标准。

    人们习惯上也是把所有针对浏览器的javascript扩展算做BOM的一部分。下面是这样的扩展
  1. 弹出新浏览器窗口的功能。
  2. 移动、缩放和关闭浏览器窗口的功能
  3. 提供浏览器详情信息的navigator对象
  4. 提供浏览器所加载页面的详细信息的location对象
  5. 提供用户显示器分辨率详细信息的screen对象
  6. 对cookie的支持
  7. 像XMLHttpRequest和IE的ActiveXObject这样的自定义对象。
