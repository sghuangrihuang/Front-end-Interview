#  前端面试题总结

#  列表
<!-- TOC -->

- [前端面试题总结](#前端面试题总结)
- [列表](#列表)
  - [web理论](#web理论)
    - [各大浏览器的内核分别是什么](#各大浏览器的内核分别是什么)
    - [介绍一下你对浏览器内核的理解？](#介绍一下你对浏览器内核的理解)
    - [前端页面有哪三层构成，分别是什么？作用是什么？](#前端页面有哪三层构成分别是什么作用是什么)
    - [讲讲输入完网址按下回车，到看到网页这个过程中发生了什么](#讲讲输入完网址按下回车到看到网页这个过程中发生了什么)
    - [谈谈你对前端性能优化的理解](#谈谈你对前端性能优化的理解)
    - [请说出三种减少页面加载时间的方法](#请说出三种减少页面加载时间的方法)
    - [列举IE与其他浏览器不一样的特性？](#列举ie与其他浏览器不一样的特性)
    - [一个页面上有大量的图片（大型电商网站），加载很慢，你有哪些方法优化这些图片的加载，给用户更好的体验。](#一个页面上有大量的图片大型电商网站加载很慢你有哪些方法优化这些图片的加载给用户更好的体验)
    - [网站重构的理解](#网站重构的理解)
    - [谈谈对“回流”的理解](#谈谈对回流的理解)
    - [线程与进程的区别](#线程与进程的区别)
    - [网页验证码是干嘛的，是为了解决什么安全问题。](#网页验证码是干嘛的是为了解决什么安全问题)
    - [什么是前端路由什么时候适合使用前端路由、前端路由有哪些优点和缺点](#什么是前端路由什么时候适合使用前端路由前端路由有哪些优点和缺点)
    - [谈谈对前端模块化的理解](#谈谈对前端模块化的理解)
    - [移动端的点击事件的有延迟，时间是多久，为什么会有？](#移动端的点击事件的有延迟时间是多久为什么会有)
    - [你如何对网站的文件和资源进行优化](#你如何对网站的文件和资源进行优化)
    - [请介绍一下渐进增强和优雅降级？](#请介绍一下渐进增强和优雅降级)
    - [什么是盒子模型？](#什么是盒子模型)
    - [一个页面从输入URL到页面加载显示完成这个过程中都发生了什么[流程说的越详细越好]](#一个页面从输入url到页面加载显示完成这个过程中都发生了什么流程说的越详细越好)
    - [是否了解公钥加密和私钥加密。](#是否了解公钥加密和私钥加密)
  - [HTML+CSS](#htmlcss)
    - [请解释一下什么是语义化的HTML](#请解释一下什么是语义化的html)
    - [HTML与XHTML——二者有什么区别](#html与xhtml二者有什么区别)
    - [img标签上title属性与alt属性的区别是什么？](#img标签上title属性与alt属性的区别是什么)
    - [如果设计中使用了非标准的字体，你该如何去实现？](#如果设计中使用了非标准的字体你该如何去实现)
    - [每个HTML文件里开头都有个很重要的东西，Doctype，知道这是干什么的吗？](#每个html文件里开头都有个很重要的东西doctype知道这是干什么的吗)
    - [你知道多少种Doctype文档类型？](#你知道多少种doctype文档类型)
    - [Doctype作用严格模式与混杂模式如何区分？它们有何意义](#doctype作用严格模式与混杂模式如何区分它们有何意义)
    - [简述一下src与href的区别](#简述一下src与href的区别)
    - [请阐述table的缺点](#请阐述table的缺点)
    - [分别写出以下几个HTML标签：文字加粗、下标、居中、字体](#分别写出以下几个html标签文字加粗下标居中字体)
    - [iframe的优缺点？](#iframe的优缺点)
    - [行内元素有哪些？块级元素有哪些？空void元素有那些？](#行内元素有哪些块级元素有哪些空void元素有那些)
    - [CSS中link和@import的区别是什么？](#css中link和import的区别是什么)
    - [对WEB标准以及W3C的理解与认识？](#对web标准以及w3c的理解与认识)
    - [说下行内元素和块级元素的区别行内块元素的兼容性使用](#说下行内元素和块级元素的区别行内块元素的兼容性使用)
    - [为什么要初始化CSS样式？](#为什么要初始化css样式)
    - [有哪项方式可以对一个DOM设置它的CSS样式？](#有哪项方式可以对一个dom设置它的css样式)
    - [什么是FOUC[无样式内容闪烁]？你如何来避免FOUC？](#什么是fouc无样式内容闪烁你如何来避免fouc)
    - [:link、:visited、:hover、:active的执行顺序是怎么样的？](#linkvisitedhoveractive的执行顺序是怎么样的)
    - [rgba和opacity的透明效果有什么不同？](#rgba和opacity的透明效果有什么不同)
    - [display:none和visibility:hidden的区别？](#displaynone和visibilityhidden的区别)
    - [对BFC规范的理解](#对bfc规范的理解)
    - [css的基本语句构成是](#css的基本语句构成是)
    - [请简述CSS的权重规则](#请简述css的权重规则)
    - [CSS优先级算法如何计算？](#css优先级算法如何计算)
    - [css属性content有什么作用？有什么应用？](#css属性content有什么作用有什么应用)
    - [line-height三种赋值方式有何区别？（带单位、纯数字、百分比）](#line-height三种赋值方式有何区别带单位纯数字百分比)
    - [position包含几种属性？absolute和relative的区别？](#position包含几种属性absolute和relative的区别)
    - [position的absolute与fixed共同点与不同点](#position的absolute与fixed共同点与不同点)
    - [请列举几种隐藏元素的方法](#请列举几种隐藏元素的方法)
    - [css如何让一段文本中的所有英文单词的首字母大写](#css如何让一段文本中的所有英文单词的首字母大写)
    - [请列举几种可以清除浮动的方法](#请列举几种可以清除浮动的方法)
    - [浏览器是怎样解析CSS选择器的？](#浏览器是怎样解析css选择器的)
    - [请简述CSS样式表继承](#请简述css样式表继承)
    - [在CSS样式中常使用px、em，各有什么优劣，在表现上有什么区别](#在css样式中常使用pxem各有什么优劣在表现上有什么区别)
    - [什么是外边距重叠？重叠的结果是什么](#什么是外边距重叠重叠的结果是什么)
    - [CSS中类class和ID的区别。](#css中类class和id的区别)
    - [请解释浮动(Float)及其工作原理。](#请解释浮动float及其工作原理)
    - [CSS伪类与CSS伪对象的区别](#css伪类与css伪对象的区别)
    - [列出display的值，说明他们的作用](#列出display的值说明他们的作用)
    - [box-sizing常用的属性有哪些分别有什么作用](#box-sizing常用的属性有哪些分别有什么作用)
    - [css中可继承的属性有哪些？](#css中可继承的属性有哪些)
    - [如何解决img下的留白？](#如何解决img下的留白)
    - [如何居中div](#如何居中div)
    - [什么是CSSHack](#什么是csshack)
    - [当float和margin同时使用时，IE6的双倍边距BUG如何解决](#当float和margin同时使用时ie6的双倍边距bug如何解决)
    - [请简述CSS的选择器](#请简述css的选择器)
    - [经常遇到的浏览器兼容性有哪些？](#经常遇到的浏览器兼容性有哪些)
    - [浮动元素引起的问题](#浮动元素引起的问题)
    - [如何使得文字不换行](#如何使得文字不换行)
    - [用纯CSS创建一个三角形的原理是什么？](#用纯css创建一个三角形的原理是什么)
    - [让页面里的字体变清晰，变细用CSS怎么做？](#让页面里的字体变清晰变细用css怎么做)
    - [如何修改chrome记住密码后自动填充表单的黄色背景？](#如何修改chrome记住密码后自动填充表单的黄色背景)
    - [font-style属性可以让它赋值为“oblique”oblique是什么意思？](#font-style属性可以让它赋值为obliqueoblique是什么意思)
    - [css多列等高如何实现？](#css多列等高如何实现)
    - [margin和padding分别适合什么场景使用？](#margin和padding分别适合什么场景使用)
    - [zoom:1的清除浮动原理](#zoom1的清除浮动原理)
    - [请说出三种减低页面加载时间的方法](#请说出三种减低页面加载时间的方法)
    - [什么是CSS预处理器和后处理器？](#什么是css预处理器和后处理器)
    - [解释下CSSsprites原理，优缺点](#解释下csssprites原理优缺点)
    - [Quirks模式是什么？它和Standards模式有什么区别？](#quirks模式是什么它和standards模式有什么区别)
  - [HTML5+CSS3](#html5css3)
    - [什么是HTML5？](#什么是html5)
    - [HTML5为什么只需要写<!Doctypehtml>](#html5为什么只需要写doctypehtml)
    - [请写出至少5个html5新增的标签，并说明其语义和应用场景](#请写出至少5个html5新增的标签并说明其语义和应用场景)
    - [html5有哪些新特性](#html5有哪些新特性)
    - [HTML5引入什么新的表单属性？](#html5引入什么新的表单属性)
    - [HTML5废弃了哪些HTML4标签](#html5废弃了哪些html4标签)
    - [哪些浏览器支持HTML5？](#哪些浏览器支持html5)
    - [HTML5的页面结构同HTML4或者更前的HTML有什么区别？](#html5的页面结构同html4或者更前的html有什么区别)
    - [除了audio和video，HTML5还有哪些媒体标签？](#除了audio和videohtml5还有哪些媒体标签)
    - [什么是响应式布局](#什么是响应式布局)
    - [响应式布局该怎么设计](#响应式布局该怎么设计)
    - [响应式布局有哪些优点和缺点](#响应式布局有哪些优点和缺点)
    - [请解释一下CSS3的Flexbox（弹性盒布局模型），以及适用场景？](#请解释一下css3的flexbox弹性盒布局模型以及适用场景)
    - [什么的媒体查询？](#什么的媒体查询)
    - [常见媒体查询有哪些？](#常见媒体查询有哪些)
    - [如何编写媒体查询？](#如何编写媒体查询)
    - [新的HTML5文档类型和字符集是？](#新的html5文档类型和字符集是)
    - [HTML5中如何嵌入音频？](#html5中如何嵌入音频)
    - [HTML5的Canvas元素有什么用？](#html5的canvas元素有什么用)
    - [HTML5存储类型有什么区别？](#html5存储类型有什么区别)
    - [label标签的作用、应用](#label标签的作用应用)
    - [如何处理HTML5新标签的浏览器兼容问题？](#如何处理html5新标签的浏览器兼容问题)
    - [如何实现浏览器内多个标签页之间的通信](#如何实现浏览器内多个标签页之间的通信)
    - [HTML5应用程序缓存和浏览器缓存有什么区别](#html5应用程序缓存和浏览器缓存有什么区别)
    - [webSocket如何兼容低浏览器](#websocket如何兼容低浏览器)
    - [HTML5的离线储存怎么使用，工作原理能不能解释一下？](#html5的离线储存怎么使用工作原理能不能解释一下)
    - [浏览器是怎么对HTML5的离线储存资源进行管理和加载的呢](#浏览器是怎么对html5的离线储存资源进行管理和加载的呢)
    - [CSS3有哪些新特性？](#css3有哪些新特性)
    - [CSS3的属性为什么要带前缀](#css3的属性为什么要带前缀)
    - [CSS3的rem单位与传统em的区别](#css3的rem单位与传统em的区别)
    - [CSS3新增伪类有那些？](#css3新增伪类有那些)
    - [before和after中双冒号和单冒号有什么区别？](#before和after中双冒号和单冒号有什么区别)
  - [JavaScript](#javascript)
    - [document。write和innerHTML的区别](#documentwrite和innerhtml的区别)
    - [javascript怎样添加、移除、移动、复制、创建节点](#javascript怎样添加移除移动复制创建节点)
    - [简述列举文档对象模型DOM里document的常用的查找访问节点的方法](#简述列举文档对象模型dom里document的常用的查找访问节点的方法)
    - [请叙述下js的基本数据类型](#请叙述下js的基本数据类型)
    - [介绍js有哪些内置对象？](#介绍js有哪些内置对象)
    - [什么是window对象什么是document对象](#什么是window对象什么是document对象)
    - [列举浏览器对象模型BOM里常用的至少4个对象，并列举window对象的常用方法至少5个](#列举浏览器对象模型bom里常用的至少4个对象并列举window对象的常用方法至少5个)
    - [BOM对象有哪些，列举window对象？](#bom对象有哪些列举window对象)
    - [谈谈对this指针的理解，可以列举几种使用情况？](#谈谈对this指针的理解可以列举几种使用情况)
    - [null和undefined的区别？](#null和undefined的区别)
    - [阐述下==和===的区别](#阐述下和的区别)
    - [面向对象的理解？](#面向对象的理解)
    - [面向对象的三大特点是什么？](#面向对象的三大特点是什么)
    - [new操作符具体干了什么呢](#new操作符具体干了什么呢)
    - [请解释一下JavaScript的同源策略](#请解释一下javascript的同源策略)
    - [如何解决跨域问题](#如何解决跨域问题)
    - [eval是做什么的？](#eval是做什么的)
    - [已知ID的Input输入框，希望获取这个输入框的输入值，怎么做？](#已知id的input输入框希望获取这个输入框的输入值怎么做)
    - [javascript函数有重载这个概念呢？](#javascript函数有重载这个概念呢)
    - [如何判断一个js对象是否是Array，最准确的方法是](#如何判断一个js对象是否是array最准确的方法是)
    - [javascript的typeof返回哪些数据类型](#javascript的typeof返回哪些数据类型)
    - [js如何获得一个DOM元素的绝对位置](#js如何获得一个dom元素的绝对位置)
    - [同步和异步的区别](#同步和异步的区别)
    - [谈谈JavaScript的作用域和作用域链](#谈谈javascript的作用域和作用域链)
    - [什么是usestrict使用它区别是什么？](#什么是usestrict使用它区别是什么)
    - [call和apply的区别是什么？](#call和apply的区别是什么)
    - [在Javascript中什么是伪数组？如何将伪数组转化为标准数组？](#在javascript中什么是伪数组如何将伪数组转化为标准数组)
    - [Javascript中callee和caller的作用？](#javascript中callee和caller的作用)
    - [JavaScript中的变量声明提升？](#javascript中的变量声明提升)
    - [请解释一下什么是闭包](#请解释一下什么是闭包)
    - [解释下JavaScript原型，原型链](#解释下javascript原型原型链)
    - [描述一下cookies，sessionStorage和localStorage的区别](#描述一下cookiessessionstorage和localstorage的区别)
    - [什么是Cookie隔离？](#什么是cookie隔离)
    - [在JavaScript中，常用的绑定事件的方法有哪些？](#在javascript中常用的绑定事件的方法有哪些)
    - [请解释什么是事件代理](#请解释什么是事件代理)
    - [javascript的事件流模型都有什么？](#javascript的事件流模型都有什么)
    - [事件是？IE与火狐的事件机制有什么区别？如何阻止冒泡？](#事件是ie与火狐的事件机制有什么区别如何阻止冒泡)
    - [谈谈对JSON的理解](#谈谈对json的理解)
    - [请你谈谈Cookie的弊端](#请你谈谈cookie的弊端)
    - [Ajax读取一个XML文档并进行解析的实例](#ajax读取一个xml文档并进行解析的实例)
    - [ajax的readystate有5个状态，每个状态表示什么？](#ajax的readystate有5个状态每个状态表示什么)
    - [Ajax有哪些好处和弊端？](#ajax有哪些好处和弊端)
    - [AJAX应用和传统Web应用有什么不同](#ajax应用和传统web应用有什么不同)
    - [Flash、Ajax各自的优缺点，在使用中如何取舍？](#flashajax各自的优缺点在使用中如何取舍)
    - [GET和POST的区别，何时使用POST？](#get和post的区别何时使用post)
    - [如何判断当前脚本运行在浏览器还是node环境中？](#如何判断当前脚本运行在浏览器还是node环境中)
    - [JS模块的封装方法，比如怎样实现私有变量，不能直接赋值，只能通过公有方法](#js模块的封装方法比如怎样实现私有变量不能直接赋值只能通过公有方法)
    - [JavaScript的值类型和引用类型](#javascript的值类型和引用类型)
    - [阐述下split与join的区别](#阐述下split与join的区别)
    - [JavaScript中，有一个函数，执行时对象查找时，永远不会去查找原型，这个函数是？](#javascript中有一个函数执行时对象查找时永远不会去查找原型这个函数是)
    - [阐述下什么是块级作用域](#阐述下什么是块级作用域)
    - [HTTP状态消息200、302、304、403、404、500分别表示什么](#http状态消息200302304403404500分别表示什么)
    - [js延迟加载的方式有哪些？](#js延迟加载的方式有哪些)
    - [requireJS的核心原理是什么？](#requirejs的核心原理是什么)
    - [内存泄露是什么，哪些操作会造成内存泄漏？](#内存泄露是什么哪些操作会造成内存泄漏)
    - [AMD、CMD规范区别？](#amdcmd规范区别)
    - [如何在页面上实现一个圆形的可点击区域？](#如何在页面上实现一个圆形的可点击区域)
    - [谈谈对ES6相对ES5增加了哪些扩展](#谈谈对es6相对es5增加了哪些扩展)
    - [ECMAScript和JavaScript的关系](#ecmascript和javascript的关系)
    - [ECMAScript6怎么写class，为什么会出现class这种东西](#ecmascript6怎么写class为什么会出现class这种东西)
    - [ECMAScript6引入了let它与传统的var有何区别？](#ecmascript6引入了let它与传统的var有何区别)
    - [谈谈对ES6const的理解](#谈谈对es6const的理解)
    - [ES6比较操作符](#es6比较操作符)
  - [jQuery](#jquery)
    - [什么是jQuery？](#什么是jquery)
    - [body中的onload函数和jQuery中jquerydocument。ready有什么区别？](#body中的onload函数和jquery中jquerydocumentready有什么区别)
    - [阐述下jquery。extend与jquery。fn。extend的区别？](#阐述下jqueryextend与jqueryfnextend的区别)
    - [阐述下bind，live，delegate的区别](#阐述下bindlivedelegate的区别)
    - [怎样才能jQuery对象与DOM对象之间的转换](#怎样才能jquery对象与dom对象之间的转换)
    - [$(this)和this关键字在jQuery中有何不同？](#this和this关键字在jquery中有何不同)
    - [jquery中get（）提交和post（）提交有区别吗？](#jquery中get提交和post提交有区别吗)
    - [jquery和javascript有什么区别？](#jquery和javascript有什么区别)
    - [jQuery与jQueryUI有啥区别？](#jquery与jqueryui有啥区别)
    - [jQuery中jquery（′class′）和jQuery中jquery('div.class')哪个效率更高？](#jquery中jquery′class′和jquery中jquerydivclass哪个效率更高)
    - [jQuery中detach（）和remove（）方法的区别是什么](#jquery中detach和remove方法的区别是什么)
    - [jQuery的slideUp动画，如果目标元素是被外部事件驱动，当鼠标快速地连续触发外部元素事件，动画会滞后的反复执行，该如何处理呢](#jquery的slideup动画如果目标元素是被外部事件驱动当鼠标快速地连续触发外部元素事件动画会滞后的反复执行该如何处理呢)
    - [在一个jQuery事件处理程序里返回了false会怎样？](#在一个jquery事件处理程序里返回了false会怎样)
    - [哪种方式更高效：document](#哪种方式更高效document)
    - [使用CDN加载jQuery库的主要优势是什么](#使用cdn加载jquery库的主要优势是什么)
    - [叙述下jQuery的特点](#叙述下jquery的特点)

<!-- /TOC -->
## web理论

### 各大浏览器的内核分别是什么

    IE: trident内核
    Firefox：gecko内核
    Safari：webkit内核
    Opera：以前是presto内核，Opera现已改用Google
    Chrome的Blink内核
    Chrome：Blink(基于webkit，Google与Opera Software共同开发)


### 介绍一下你对浏览器内核的理解？

    主要分成两部分：渲染引擎和JS引擎。
    渲染引擎：负责取得网页的内容（HTML、XML、图像等等）、整理讯息（例如加入CSS等），以及计算网页的显示方式，然后会输出至显示器或打印机。浏览器的内核的不同对于网页的语法解释会有不同，所以渲染的效果也不相同。所有网页浏览器、电子邮件客户端以及其它需要编辑、显示网络内容的应用程序都需要内核。
    JS引擎：解析和执行javascript来实现网页的动态效果。
    最开始渲染引擎和JS引擎并没有区分的很明确，后来JS引擎越来越独立，内核就倾向于只指渲染引擎。

### 前端页面有哪三层构成，分别是什么？作用是什么？

    1)结构层：由 HTML 或 XHTML 之类的标记语言负责创建，仅负责语义的表达。解决了页面“内容是什么”的问题。
    2)表示层：由CSS负责创建，解决了页面“如何显示内容”的问题。
    3)行为层：由脚本负责。解决了页面上“内容应该如何对事件作出反应”的问题。

### 讲讲输入完网址按下回车，到看到网页这个过程中发生了什么

    a. 域名解析
    b. 发起TCP的3次握手
    c. 建立TCP连接后发起http请求
    d. 服务器端响应http请求，浏览器得到html代码
    e. 浏览器解析html代码，并请求html代码中的资源
    f. 浏览器对页面进行渲染呈现给用户

### 谈谈你对前端性能优化的理解

    a. 请求数量：合并脚本和样式表，CSS Sprites，拆分初始化负载，划分主域
    b. 请求带宽：开启GZip，精简JavaScript，移除重复脚本，图像优化，将icon做成字体
    c. 缓存利用：使用CDN，使用外部JavaScript和CSS，添加Expires头，减少DNS查找，配置ETag，使AjaX可缓存
    d. 页面结构：将样式表放在顶部，将脚本放在底部，尽早刷新文档的输出
    e. 代码校验：避免CSS表达式，避免重定向

### 请说出三种减少页面加载时间的方法

    a.优化图片
    b.图像格式的选择（GIF：提供的颜色较少，可用在一些对颜色要求不高的地方）
    c.优化CSS（压缩合并css，如margin-top,margin-left...)
    d.网址后加斜杠（如www.campr.com/目录，会判断这个“目录是什么文件类型，或者是目录。）
    e.标明高度和宽度（如果浏览器没有找到这两个参数，它需要一边下载图片一边计算大小，如果图片很多，浏览器需要不断地调整页面。这不但影响速度，也影响浏览体验。
    当浏览器知道了高度和宽度参数后，即使图片暂时无法显示，页面上也会腾出图片的空位，然后继续加载后面的内容。从而加载时间快了，浏览体验也更好了。）
    f.减少http请求（合并文件，合并图片）

### 列举IE与其他浏览器不一样的特性？

    a. IE的排版引擎是Trident （又称为MSHTML）
    b. Trident内核曾经几乎与W3C标准脱节（2005年）
    c. Trident内核的大量 Bug等安全性问题没有得到及时解决
    d. JS方面，有很多独立的方法，例如绑定事件的attachEvent、创建事件的createEventObject等
    e. CSS方面，也有自己独有的处理方式，例如设置透明，低版本IE中使用滤镜的方式

### 一个页面上有大量的图片（大型电商网站），加载很慢，你有哪些方法优化这些图片的加载，给用户更好的体验。

    a. IE的排版引擎是Trident （又称为MSHTML）
    b. Trident内核曾经几乎与W3C标准脱节（2005年）
    c. Trident内核的大量 Bug等安全性问题没有得到及时解决
    d. JS方面，有很多独立的方法，例如绑定事件的attachEvent、创建事件的createEventObject等
    e. CSS方面，也有自己独有的处理方式，例如设置透明，低版本IE中使用滤镜的方式

### 网站重构的理解

    重构：在不改变外部行为的前提下，简化结构、添加可读性，而在网站前端保持一致的行为。
    a. 使网站前端兼容于现代浏览器(针对于不合规范的CSS、如对IE6有效的)
    b. 对于移动平台的优化，针对于SEO进行优化OM
    c. 减少代码间的耦合，让代码保持弹性
    d. 压缩或合并JS、CSS、image等前端资源

### 谈谈对“回流”的理解

    回流指的是浏览器为了重新渲染页面的需要而进行的重新计算元素的几何大小和位置的，他的开销是非常大的，回流可以理解为渲染树需要重新进行计算，一般最好触发元素的重构，避免元素的回流；比如通过通过添加类来添加css样式，而不是直接在DOM上设置，当需要操作某一块元素时候，最好使其脱离文档流，这样就不会引起回流了，比如设置position：absolute或者fixed，或者display：none，等操作结束后在显示、

### 线程与进程的区别

    一个程序至少有一个进程,一个进程至少有一个线程.
    线程的划分尺度小于进程，使得多线程程序的并发性高。
    另外，进程在执行过程中拥有独立的内存单元，而多个线程共享内存，从而极大地提高了程序的运行效率。
    线程在执行过程中与进程还是有区别的。每个独立的线程有一个程序运行的入口、顺序执行序列和程序的出口。
    但是线程不能够独立执行，必须依存在应用程序中，由应用程序提供多个线程执行控制。
    从逻辑角度来看，多线程的意义在于一个应用程序中，有多个执行部分可以同时执行。但操作系统并没有将多个线程看做多个独立的应用，来实现进程的调度和管理以及资源分配。

### 网页验证码是干嘛的，是为了解决什么安全问题。

    区分用户是计算机还是人的公共全自动程序。可以防止恶意破解密码、刷票、论坛灌水；有效防止黑客对某一个特定注册用户用特定程序暴力破解方式进行不断的登陆尝试。

### 什么是前端路由什么时候适合使用前端路由、前端路由有哪些优点和缺点

    前端路由就是把不同路由对应不同的内容或页面的任务交给前端来做，之前是通过服务端根据 url 的不同返回不同的页面实现的。
    适合使用：在单页面应用，大部分页面结构不变，只改变部分内容的使用
    前端路由有什么优点和缺点？
    用户体验好，不需要每次都从服务器全部获取，快速展现给用户，但使用浏览器的前进，后退键的时候会重新发送请求，没有合理地利用缓存，单页面无法记住之前滚动的位置，无法在前进，后退的时候记住滚动的位置。

### 谈谈对前端模块化的理解

    前端模块话就是把复杂的文件分成一个个独立的模块，比如js文件，分成独立的模块之后有利于代码的重用和维护，但是这样又会引来模块与模块之间的依赖问题，所以就有了CommonJS、AMD、CMD规范，最后出现了webpack，webpack就是前端模块话的一种解决方案，基本上大公司都会使用webpack等

### 移动端的点击事件的有延迟，时间是多久，为什么会有？ 

    由于两次连续“轻触”是“放大”的操作（即使你两次轻触的是一个链接或一个有click事件监听器的元素），所以在第一次被“轻触”后，浏览器需要先等一段时间，看看有没有所谓的“连续的第二次轻触”。如果有，则进行“放大”操作。没有，才敢放心地认为用户不是要放大，而是需要“click”至此才敢触发click事件，导致“短按（手指接触屏幕到离开屏幕的时间比较短）”的click事件通常约会延迟300ms左右。

### 你如何对网站的文件和资源进行优化

    期待的解决方案包括：
    1)文件合并
    2)文件最小化/文件压缩
    3)使用CDN托管
    4)缓存的使用

### 请介绍一下渐进增强和优雅降级？

    渐进增强： 针对低版本浏览器进行构建页面，保证最基本的功能，然后再针对高级浏览器进行效果、交互等改进和追加功能达到更好的用户体验。
    优雅降级 ： 一开始就构建完整的功能，然后再针对低版本浏览器进行兼容。
    两者之间区别：
    a. 优雅降级是从复杂的现状开始，并试图减少用户体验的供给;
    b. 渐进增强则是从一个非常基础的，能够起作用的版本开始，并不断扩充，以适应未来环境的需要;
    c. 降级（功能衰减）意味着往回看；而渐进增强则意味着朝前看，同时保证其根基处于安全地带;

### 什么是盒子模型？

    在网页中，一个元素占有空间的大小由几个部分构成，其中包括元素的内容（content），元素的内边距（padding），元素的边框（border），元素的外边距（margin）四个部分。
    这四个部分占有的空间中，有的部分可以显示相应的内容，而有的部分只用来分隔相邻的区域或区域。4个部分一起构成了css中元素的盒模型。

### 一个页面从输入URL到页面加载显示完成这个过程中都发生了什么[流程说的越详细越好]

    简洁版：
    浏览器根据请求的URL交给DNS域名解析，找到真实IP，向服务器发起请求；
    服务器交给后台处理完成后返回数据，浏览器接收文件（HTML、JS、CSS、图象等）；
    浏览器对加载到的资源（HTML、JS、CSS等）进行语法解析，建立相应的内部数据结构（如HTML的DOM）；
    载入解析到的资源文件，渲染页面，完成。
    详细版：
    1、浏览器会开启一个线程来处理这个请求，对 URL 分析判断如果是 http 协议就按照 Web 方式来处理;
    2、调用浏览器内核中的对应方法，比如 WebView 中的 loadUrl 方法;
    3、通过DNS解析获取网址的IP地址，设置 UA 等信息发出第二个GET请求;
    4、进行HTTP协议会话，客户端发送报头(请求报头);
    5、进入到web服务器上的 Web Server，如 Apache、Tomcat、Node.JS 等服务器;
    6、进入部署好的后端应用，如 PHP、Java、JavaScript、Python 等，找到对应的请求处理;
    7、处理结束回馈报头，此处如果浏览器访问过，缓存上有对应资源，会与服务器最后修改时间对比，一致则返回304;
    8、浏览器开始下载html文档(响应报头，状态码200)，同时使用缓存;
    9、文档树建立，根据标记请求所需指定MIME类型的文件（比如css、js）,同时设置了cookie;
    10、页面开始渲染DOM，JS根据DOM API操作DOM,执行事件绑定等，页面显示完成。

### 是否了解公钥加密和私钥加密。

    一般情况下是指私钥用于对数据进行签名，公钥用于对签名进行验证;
    HTTP网站在浏览器端用公钥加密敏感数据，然后在服务器端再用私钥解密。


---

##  HTML+CSS

### 请解释一下什么是语义化的HTML

    语义化的HTML使用每个html标签都特定的用途，例如p标签常用于文章段落，h1~h6常用于标题，strong字体加粗强调….。
    语义化的好处：
    1)去掉或样式丢失的时候能让页面呈现清晰的结构：
        html本身是没有表现的，我们看到例如<h1>是粗体，字体大小2em，加粗；<strong>是加粗的，不要认为这是html的表现，这些其实html默认的css样式在起作用，所以去掉或样式丢失的时候能让页面呈现清晰的结构不是语义化的HTML结构的优点，但是浏览器都有有默认样式，默认样式的目的也是为了更好的表达html的语义，可以说浏览器的默认样式和语义化的HTML结构是不可分割的。
    2)屏幕阅读器（如果访客有视障）会完全根据你的标记来“读”你的网页.
    3)搜索引擎的爬虫也依赖于标记来确定上下文和各个关键字的权重.
    4)你的页面是否对爬虫容易理解非常重要,因为爬虫很大程度上会忽略用于表现的标记,而只注重语义标记.
    5)便于团队开发和维护

### HTML与XHTML——二者有什么区别

    HTML是一种基本的WEB网页设计语言，
    XHTML是一个基于XML的置标语言
    区别：
    1)XHTML 元素必须被正确地嵌套。
    2)XHTML 元素必须被关闭。空标签也必须被关闭，如<br>必须换成<br/>
    3)标签名必须用小写字母。
    4)XHTML 文档必须拥有根元素。
    5)XHTML要求给所有属性一个值
    6)XHTML要求所有的属性必须用引号""括起来
    7)XHTML 文档需要把所有 < 、>、& 等特殊符号用编码表示
    8)XHTML 文档不要在注释内容中使“--”
    9)XHTML 图片必须有说明文字
    10)XHTML 文档中用id属性代替name属性

### img标签上title属性与alt属性的区别是什么？

    alt属性是为了给那些不能看到你文档中图像的浏览者提供文字说明的。且长度必须少于100个英文字符或者用户必须保证替换文字尽可能的短。这包括那些使用本来就不支持图像显示或者图像显示被关闭的浏览器的用户，视觉障碍的用户和使用屏幕阅读器的用户等。
    title属性为设置该属性的元素提供建议性的信息。使用title属性提供非本质的额外信息。

### 如果设计中使用了非标准的字体，你该如何去实现？

    1)用图片代替  2)使用在线字库。

### 每个HTML文件里开头都有个很重要的东西，Doctype，知道这是干什么的吗？

    <!DOCTYPE> 声明位于文档中的最前面的位置，处于 <html> 标签之前。
    此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范。（重点：告诉浏览器按照何种规范解析页面）

### 你知道多少种Doctype文档类型？

    标签可声明三种 DTD 类型，分别表示严格版本、过渡版本以及基于框架的 HTML 文档。
    HTML 4.01 规定了三种文档类型：Strict、Transitional 以及 Frameset。
    XHTML 1.0 规定了三种 XML 文档类型：Strict、Transitional 以及 Frameset。
    Standards （标准）模式（也就是严格呈现模式）用于呈现遵循最新标准的网页，
    Quirks（包容）模式（也就是松散呈现模式或者兼容模式）用于呈现为传统浏览器而设计的网页。

### Doctype作用严格模式与混杂模式如何区分？它们有何意义

    声明位于文档中的最前面，处于html标签之前。告知浏览器以何种模式来渲染文档。
    严格模式的排版和 JS 运作模式是，以该浏览器支持的最高标准运行。
    在混杂模式中，页面以宽松的向后兼容的方式显示。模拟老式浏览器的行为以防止站点无法工作。
    DOCTYPE不存在或格式不正确会导致文档以混杂模式呈现。

### 简述一下src与href的区别

    src用于替换当前元素；href用于在当前文档和引用资源之间确立联系。
    src是source的缩写，指向外部资源的位置，指向的内容将会嵌入到文档中当前标签所在位置，在请求src资源时会将其指向的资源下载并应用到当前文档中，例如js脚本，img图片和frame等元素。
    href是Hypertext Reference的缩写，指向网络资源所在位置，建立和当前元素（锚点）或当前文档（链接）之间的链接。


### 请阐述table的缺点

    1)太深的嵌套，比如table>tbody>tr>td>h3，会导致搜索引擎读取困难，而且，最直接的损失就是大大增加了冗余代码量。
    2)灵活性差，比如要将tr设置border等属性，是不行的，得通过td
    3)代码臃肿，当在table中套用table的时候，阅读代码会显得异常混乱
    4)混乱的colspan与rowspan，用来布局时，频繁使用他们会造成整个文档顺序混乱。
    5)不够语义

### 分别写出以下几个HTML标签：文字加粗、下标、居中、字体

    加粗：<b>、<strong>
    下标：<sub>
    居中：<center>
    字体：<font>、<basefont>

### iframe的优缺点？

    优点：
    a. 解决加载缓慢的第三方内容如图标和广告等的加载问题
    b. iframe无刷新文件上传
    c. iframe跨域通信
    缺点：
    a. iframe会阻塞主页面的Onload事件
    b. 无法被一些搜索引擎索引到
    c. 页面会增加服务器的http请求
    d. 会产生很多页面，不容易管理。

### 行内元素有哪些？块级元素有哪些？空void元素有那些？

    行内元素：a、b、span、img、input、strong、select、label、em、button、textarea等等
    块级元素：div、ul、li、dl、dt、dd、p、h1-h6、blockquote
    空元素：即系没有内容的HTML元素，例如：br、meta、hr、link、input、img

### CSS中link和@import的区别是什么？

    a. link属于HTML标签，而@import是CSS提供的，且只能加载 CSS
    b. 页面被加载时，link会同时被加载，而@import引用的CSS会等到页面被加载完再加载
    c. import只在IE5以上才能识别，而link是HTML标签，无兼容问题
    d. link方式的样式的权重 高于@import的权重
    e. 当使用 Javascript 控制 DOM 去改变样式的时候，只能使用 link 方式，因为 @import 眼里只有 CSS ，不是 DOM 可以控制

### 对WEB标准以及W3C的理解与认识？

    （1）web标准规范要求，书写标签必须闭合、标签小写、不乱嵌套，可提高搜索机器人对网页内容的搜索几率；
    （2）建议使用外链css和js脚本，从而达到结构与行为、结构与表现的分离，提高页面的渲染速度，能更快地显示页面的内容；
    （3）样式与标签的分离，更合理的语义化标签，使内容能被更多的用户所访问、内容能被更广泛的设备所访问、更少的代码和组件， 从而降低维护成本、改版更方便；
    （4）不需要变动页面内容，便可提供打印版本而不需要复制内容，提高网站易用性；遵循w3c制定的web标准，能够使用户浏览者更方便的阅读，使网页开发者之间更好的交流。

### 说下行内元素和块级元素的区别行内块元素的兼容性使用

    行内元素：会在水平方向排列，不能包含块级元素，设置width无效，height无效(可以设置line-height，margin上下无效，padding上下无效。
    块级元素：各占据一行，垂直方向排列。从新行开始结束接着一个断行。 兼容性：display:inline-block;display:inline;zoom:1;

### 为什么要初始化CSS样式？

    因为浏览器的兼容问题，不同浏览器对有些标签的默认值是不同的，如果没对CSS初始化往往会出现浏览器之间的页面显示差异。当然，初始化样式会对SEO有一定的影响，但鱼和熊掌不可兼得，但力求影响最小的情况下初始化。
    最简单的初始化方法就是 *{padding: 0; margin: 0;}

### 有哪项方式可以对一个DOM设置它的CSS样式？

    a. 外部样式表：通过<link>标签引入一个外部css文件
    b. 内部样式表：将css代码放在 <style> 标签内部
    c. 内联样式：将css样式直接定义在 HTML 元素内部

### 什么是FOUC[无样式内容闪烁]？你如何来避免FOUC？

    如果使用import方法对CSS进行导入，会导致某些页面在Windows下的IE出现一些奇怪的现象：
    以无样式显示页面内容的瞬间闪烁，这种现象称之为文档样式短暂失效，简称为FOUC。
    原理：
    当样式表晚于结构性html加载，当加载到此样式表时，页面将停止之前的渲染。此样式表被下载和解析后，将重新渲染页面，也就出现了短暂的花屏现象。
    解决方法：
    使用LINK标签将样式表放在文档HEAD中。


### :link、:visited、:hover、:active的执行顺序是怎么样的？

    L-V-H-A，l(link)ov(visited)e h(hover)a(active)te，即用喜欢和讨厌两个词来概括

### rgba和opacity的透明效果有什么不同？

    a. opacity作用于元素，以及元素内的所有内容的透明度，rgba()只作用于元素的颜色或其背景色。
    b. 设置rgba透明的元素的子元素不会继承透明效果！

### display:none和visibility:hidden的区别？

    display:none  隐藏对应的元素，在文档布局中不再给它分配空间，它各边的元素会合拢，就当他从来不存在。
    visibility:hidden  隐藏对应的元素，但是在文档布局中仍保留原来的空间。

### 对BFC规范的理解

    BFC，块级格式化上下文，一个创建了新的BFC的盒子是独立布局的，盒子里面的子元素的样式不会影响到外面的元素。
    在同一个BFC中的两个毗邻的块级盒在垂直方向（和布局方向有关系）的margin会发生折叠。   

### css的基本语句构成是

    选择器{属性1:值1;属性2:值2;……}

### 请简述CSS的权重规则

    一个行内样式+1000，一个id+100，一个属性选择器/class类/伪类选择器+10，一个元素名/伪对象选择器+1。
    关系选择器将拆分为两个选择器再计算.

### CSS优先级算法如何计算？

    优先级就近原则，同权重情况下样式定义最近者为准;  载入样式以最后载入的定位为准;
    优先级为:
    同权重: 内联样式表（标签内部）> 嵌入样式表（当前文件中）> 外部样式表（外部文件中）。
    !important >  id > class > tag
    important 比 内联优先级高

### css属性content有什么作用？有什么应用？

    css的content属性专门应用在 before/after 伪元素上，用于来插入生成内容。可以配合自定义字体显示特殊符号。

### line-height三种赋值方式有何区别？（带单位、纯数字、百分比）

    带单位：px不用计算，em则会使元素以其父元素font-size值为参考来计算自己的行高
    纯数字：把比例传递给后代，例如父级行高为1.5，子元素字体为18px，则子元素行高为1.5*18=27px
    百分比：将计算后的值传递给后代


### position包含几种属性？absolute和relative的区别？

    static：默认状态、没有定位、正常流
    inherit：从父元素集成position属性的值
    fixed：生成绝对定位的元素（相对于浏览器窗口进行定位）
    absolute：生成绝对定位的元素（相位与static定位以外的第一个父元素定位）
    relative：生成相对定位的元素（相对于其正常位置定位）
    absolute和relative区别：父元素的padding对relative的子元素布局有影响，absolute的子元素不受影响

### position的absolute与fixed共同点与不同点

    相同：
        a. 改变行内元素的呈现方式，display被置为block	
        b. 让元素脱离普通流，不占据空间
        c. 默认会覆盖到非定位元素上
    区别：
        absolute的”根元素“是可以设置的，而fixed的”根元素“固定为浏览器窗口。
        当你滚动网页，fixed元素与浏览器窗口之间的距离是不变的。

### 请列举几种隐藏元素的方法

    a. visibility: hidden；这个属性只是简单的隐藏某个元素，但是元素占用的空间任然存在。
    b. opacity: 0；一个CSS3属性，设置0可以使一个元素完全透明，制作出和visibility一样的效果。与visibility相比，它可以被transition和animate
    c. position:absolute；使元素脱离文档流，处于普通文档之上，给它设置一个很大的left负值定位，使元素定位在可见区域之外。
    d. display: none；元素会变得不可见，并且不会再占用文档的空间。
    e. transform: scale(0)；将一个元素设置为无限小，这个元素将不可见。这个元素原来所在的位置将被保留。
    f. HTML5 hidden attribute；hidden属性的效果和display:none;相同，这个属性用于记录一个元素的状态
    g. height:0;overflow:hidden；将元素在垂直方向上收缩为0使元素消失。只要元素没有可见的边框，该技术就可以正常工作。
    h. filter: blur(0)；将一个元素的模糊度设置为0，从而使这个元素“消失”在页面中。

### css如何让一段文本中的所有英文单词的首字母大写

    text-transform：none| capitalize(将每个单词的第一个字母转换成大写) | uppercase(将每个单词转换成大写 ) | lowercase(将每个单词转换成小写 )

### 请列举几种可以清除浮动的方法

    浮动会漂浮于普通流之上，像浮云一样，但是只能左右浮动。正是这种特性，导致框内部由于不存在其他普通流元素了，表现出高度为0（高度塌陷）。
    a. 添加额外标签，例如<div style="clear:both"></div>
    b. 使用br标签和其自身的html属性，例如<br clear="all" />
    c. 父元素设置 overflow：hidden；在IE6中还需要触发hasLayout，例如zoom：1；
    d. 父元素设置 overflow：auto 属性；同样IE6需要触发hasLayout
    e. 父元素也设置浮动
    f. 父元素设置display:table
    g. 使用:after 伪元素；由于IE6-7不支持:after，使用 zoom:1触发 hasLayout。

### 浏览器是怎样解析CSS选择器的？

    样式系统从关键选择器开始匹配，然后左移查找规则选择器的祖先元素。
    只要选择器的子树一直在工作，样式系统就会持续左移，直到和规则匹配，或者是因为不匹配而放弃该规则。

### 请简述CSS样式表继承

    CSS样式表继承指的是，特定的CSS属性向下传递到子孙元素。会被继承下去的属性如下：
    文本相关：font-family，font-size， font-style，font-variant，font-weight， font，letter-spacing，line-height，color
    列表相关：list-style-image，list-style-position，list-style-type， list-style

### 在CSS样式中常使用px、em，各有什么优劣，在表现上有什么区别

    px是相对长度单位，相对于显示器屏幕分辨率而言的。px定义的字体，无法用浏览器字体放大功能。
    em是相对长度单位，相对于当前对象内文本的字体尺寸。em的值并不是固定的，会继承父级元素的字体大小，1 ÷ 父元素的font-size × 需要转换的像素值 = em值。

### 什么是外边距重叠？重叠的结果是什么

    在CSS当中，相邻的两个盒子（可能是兄弟关系也可能是祖先关系）的外边距可以结合成一个单独的外边距。这种合并外边距的方式被称为折叠，并且因而所结合成的外边距称为折叠外边距。
    重叠的结果就是这个外边距高度等于两个发生层叠的外边距的高度中的较大者。

### CSS中类class和ID的区别。

    1)书写上的差别：class名用“.”号开头来定义，id名用“#”号开头来定义；
	2)调用上的区别：在同一个html网页页面中class是可以被多次调用的（在不同的地方）。而id名作为标签的身份则是唯一的，id在页面中只能出现一次。在js脚本中经常会用到id来修改一个标签的属性
	3)id作为元素的标签，用于区分不同结构和内容，而class作为一个样式，它可以应用到任何结构和内容上。
	4)在布局思路上，一般坚持这样的原则：id是先确定页面的结构和内容，然后再为它定义样式：而class相反，它先定义好一类样式，然后再页面中根据需要把类样式应用到不同的元素和内容上面。
	5)在实际应用时，class更多的被应用到文字版块以及页面修饰等方面，而id更多地被用来实现宏伟布局和设计包含块，或包含框的样式。

### 请解释浮动(Float)及其工作原理。

    float属性定义了元素是否浮动及在哪个方向浮动，在CSS中任何元素都可以浮动，且浮动元素会生成一个块级框，而不论它本身是何种元素。并且盒子的宽度不在伸展，而是根据盒子里面的内容的宽度来确定。浮动属性会使得浮动的元素脱离文档流，所以文档的普通流中的块框会表现的像浮动框不存在一样

### CSS伪类与CSS伪对象的区别

    CSS引入伪类和伪元素的概念是为了描述一些现有CSS无法描述的东西根本区别在于：它们是否创造了新的元素（抽象）
    伪类：一开始用来表示一些元素的动态状态，随后CSS2标准扩展了其概念范围，使其成为了所有逻辑上存在但在文档树中却无须标识的“幽灵”分类
    伪对象：代表了某个元素的子元素，这个子元素虽然在逻辑上存在，但却并不实际存在于文档树中

### 列出display的值，说明他们的作用

    block         块类型。默认宽度为父元素宽度，可设置宽高，换行显示。
    none          缺省值。象行内元素类型一样显示。
    inline        行内元素类型。默认宽度为内容宽度，不可设置宽高，同行显示。
    inline-block  默认宽度为内容宽度，可以设置宽高，同行显示。
    list-item     象块类型元素一样显示，并添加样式列表标记。
    table         此元素会作为块级表格来显示。
    inherit       规定应该从父元素继承 display 属性的值。

### box-sizing常用的属性有哪些分别有什么作用

    常用的属性：box-sizing: content-box border-box
    作用：
    content-box:宽度和高度分别应用到元素的内容框。在宽度和高度之外绘制元素的内边距和边框(元素默认效果)。
    border-box:元素指定的任何内边距和边框都将在已设定的宽度和高度内进行绘制。通过从已设定的宽度和高度分别减去边框和内边距才能得到内容的宽度和高度。

### css中可继承的属性有哪些？

    font-size font-family color 等等

### 如何解决img下的留白？

    产生原因	
    Img元素是行内元素，图片默认的vertical-align样式是baseline 也就是说图片放置在父元素的基线上。
    解决方案
    1)给img设定 display:block样式 （将使 img 超出文字基线，致使空白消失。）
    2)设置图片的垂直对齐方式 （将使 img 超出文字基线，致使空白消失。）
    设置图片的vertical-align属性为“top，text-top，bottom，text-bottom”
    3)设置父对象的文字大小为0px （用于行内没有其他元素）
    4)设置图片的浮动属性  (如果要实现图文混排，这种方法是很好的选择)

### 如何居中div

    1、给div 设置一个宽度，然后添加 margin:0 auto 属性
    2、父类text-align:center；div设置宽度+设置行内块状

### 什么是CSSHack

    一般来说是针对不同的浏览器写不同的CSS，就是CSSHack。
    IE浏览器Hack一般又分为三种，条件Hack、属性级Hack、选择符Hack
    // 1、条件Hack
    <!--[if IE]>
    <style>
        .test{color:red;}
    </style>
    <![endif]-->
    // 2、属性Hack
    .test{
        color:#090\9; /* For IE8+ */
        *color:#f00;  /* For IE7 and earlier */
        _color:#ff0;  /* For IE6 and earlier */
    }
    // 3、选择符Hack
    * html .test{color:#090;}       /* For IE6 and earlier */
    * + html .test{color:#ff0;}     /* For IE7 */

### 当float和margin同时使用时，IE6的双倍边距BUG如何解决

    display：inline;或者margin-right:-3px;

### 请简述CSS的选择器

    元素选择器：* 、E、 E#id、 E.class
    关系选择器：E、F、E>F、E+F、E~F
    属性选择器：E[att]、E[att="val"]、E[att~="val"]、E[att^="val"]、E[att$="val"]、E[att*="val"]、E[att|="val"]
    伪类选择器：E:link、E:visited、E:hover、E:active、E:focus、E:lang(fr)、E:not(s)、E:root、E:first-child、E:last-chil等
    伪对象选择器：E:first-letter/E::first-letter、E:first-line/E::first-line、E:before/E::before、E:after/E::after、E::selection

### 经常遇到的浏览器兼容性有哪些？

	a. 浏览器默认的margin和padding不同
	b. IE6双边距bug
	c. 在ie6，ie7中元素高度超出自己设置高度。原因是IE8以前的浏览器中会给元素设置默认的行高的高度导致的
	d. min-height在IE6下不起作用
	e. 透明性IE用filter:Alpha(Opacity=60)，而其他主流浏览器用 opacity:0.6
	f. input边框问题，去掉input边框一般用border:none;就可以，但由于IE6在解析input样式时的BUG(优先级问题)，在IE6下无效移除空格，使用margin 负值、使用 font-size:0、letter-spacing 、word-spacing


### 浮动元素引起的问题

	a. 父元素的高度无法被撑开，影响与父元素同级的元素
	b. 与浮动元素同级的非浮动元素会跟随其后
	c. 若非第一个元素浮动，则该元素之前的元素也需要浮动，否则会影响页面显示的结构

### 如何使得文字不换行

    定义包含文字的容器为：
    width:xxx;white-space:nowrap;text-overflow: ellipsis;（以省略号结尾）
    53、 如何使得英文单词不发生词内断行？
    word-wrap:break-word;

### 用纯CSS创建一个三角形的原理是什么？

    设置边框把上、左、右三边隐藏掉（颜色设为 transparent）
    #demo {
        width: 0;
        height: 0;
        border-width: 20px;
        border-style: solid;
        border-color: transparent transparent red transparent;
    }

### 让页面里的字体变清晰，变细用CSS怎么做？

    -webkit-font-smoothing: antialiased;

### 如何修改chrome记住密码后自动填充表单的黄色背景？

    input:-webkit-autofill, textarea:-webkit-autofill, select:-webkit-autofill {
        background-color: rgb(250, 255, 189); /* #FAFFBD; */
        background-image: none;
        color: rgb(0, 0, 0);
    }

### font-style属性可以让它赋值为“oblique”oblique是什么意思？

    倾斜的字体样式

### css多列等高如何实现？

    利用padding-bottom|margin-bottom正负值相抵；
    设置父容器设置超出隐藏（overflow:hidden），这样子父容器的高度就还是它里面的列没有设定padding-bottom时的高度，
    当它里面的任 一列高度增加了，则父容器的高度被撑到里面最高那列的高度，
    其他比这列矮的列会用它们的padding-bottom补偿这部分高度差。

### margin和padding分别适合什么场景使用？

    margin是用来隔开元素与元素的间距；padding是用来隔开元素与内容的间隔。
    margin用于布局分开元素使元素与元素互不相干；
    padding用于元素与内容之间的间隔，让内容（文字）与（包裹）元素之间有一段

### zoom:1的清除浮动原理

    清除浮动，触发hasLayout；
    Zoom属性是IE浏览器的专有属性，它可以设置或检索对象的缩放比例。解决ie下比较奇葩的bug。
    譬如外边距（margin）的重叠，浮动清除，触发ie的haslayout属性等。
    来龙去脉大概如下：
    当设置了zoom的值之后，所设置的元素就会就会扩大或者缩小，高度宽度就会重新计算了，这里一旦改变zoom值时其实也会发生重新渲染，运用这个原理，也就解决了ie下子元素浮动时候父元素不随着自动扩大的问题。
    Zoom属是IE浏览器的专有属性，火狐和老版本的webkit核心的浏览器都不支持这个属性。然而，zoom现在已经被逐步标准化，出现在 CSS 3.0 规范草案中。
    目前非ie由于不支持这个属性，它们又是通过什么属性来实现元素的缩放呢？可以通过css3里面的动画属性scale进行缩放。

### 请说出三种减低页面加载时间的方法

    1)压缩css、js文件
    2)合并js、css文件，减少http请求
    3)外部js、css文件放在最底下
    4)减少dom操作，尽可能用变量替代不必要的dom操作 

### 什么是CSS预处理器和后处理器？

    - 预处理器例如：LESS、Sass、Stylus，用来预编译Sass或less，增强了css代码的复用性，还有层级、mixin、变量、循环、函数等，具有很方便的UI组件模块化开发能力，极大的提高工作效率。
    后处理器例如：PostCSS，通常被视为在完成的样式表中根据CSS规范处理CSS，让其更有效；
    目前最常做的是给CSS属性添加浏览器私有前缀，实现跨浏览器兼容性的问题。

### 解释下CSSsprites原理，优缺点

    CSS Sprites其实就是把网页中一些背景图片整合到一张图片文件中，再利用CSS的“background-image”，“background- repeat”，“background-position”的组合进行背景定位，background-position可以用数字精确的定位出背景图片的位置。
    优点：
	a. 减少网页的http请求
	b. 减少图片的字节
	c. 解决了网页设计师在图片命名上的困扰，只需对一张集合的图片上命名就可以了，不需要对每一个小元素进行命名
	d. 更换风格方便，只需要在一张或少张图片上修改图片的颜色或样式，整个网页的风格就可以改变。
    缺点：
	a. 在宽屏，高分辨率的屏幕下的自适应页面，你的图片如果不够宽，很容易出现背景断裂
	b. CSS Sprites在开发的时候，要通过photoshop或其他工具测量计算每一个背景单元的精确位置
	c. 在维护的时候比较麻烦，如果页面背景有少许改动，一般就要改这张合并的图片


### Quirks模式是什么？它和Standards模式有什么区别？

    在写程序时我们也会经常遇到这样的问题，如何保证原来的接口不变，又提供更强大的功能，尤其是新功能不兼容旧功能时。IE6以前的页面大家都不会去写DTD，所以IE6就假定 如果写了DTD，就意味着这个页面将采用对CSS支持更好的布局，而如果没有，则采用兼容之前的布局方式。这就是Quirks模式（怪癖模式，诡异模式，怪异模式）。
	区别：总体会有布局、样式解析和脚本执行三个方面的区别。
	a. 盒模型：在W3C标准中，如果设置一个元素的宽度和高度，指的是元素内容的宽度和高度，而在Quirks 模式下，IE的宽度和高度还包含了padding和border。
	b. 设置行内元素的高宽：在Standards模式下，给等行内元素设置wdith和height都不会生效，而在quirks模式下，则会生效。
	c. 设置百分比的高度：在standards模式下，一个元素的高度是由其包含的内容来决定的，如果父元素没有设置百分比的高度，子元素设置一个百分比的高度是无效的用
	d. 设置水平居中：使用margin:0 auto在standards模式下可以使元素水平居中，但在quirks模式下却会失效。


---

##  HTML5+CSS3

    

### 什么是HTML5？

    HTML5 是对 HTML 标准的第五次修订。其主要的目标是将互联网语义化，以便更好地被人类和机器阅读，并同时提供更好地支持各种媒体的嵌入。HTML5 的语法是向后兼容的。 HTML5将会取代99年制定的HTML 4.01、XHTML 1.0标准，以期能在互联网应用迅速发展的时候，使网络标准达到符合当代的网络需求，为桌面和移动平台带来无缝衔接的丰富内容。
    HTML5的设计目的是为了在移动设备上支持多媒体。新的语法特征被引进以支持这一点，如video、audio和canvas 标记。

### HTML5为什么只需要写<!Doctypehtml>

    HTML5不基于 SGML，因此不需要对DTD进行引用;但是需要doctype来规范浏览器的行为(让浏览器按照它们应该的方式来运行)。而HTML4.01基于SGML,所以需要对DTD进行引用，才能告知浏览器文档所使用的文档类型。

### 请写出至少5个html5新增的标签，并说明其语义和应用场景

    section：定义文档中的一个章节
    nav：定义只包含导航链接的章节
    header：定义页面或章节的头部。它经常包含 logo、页面标题和导航性的目录。
    footer：定义页面或章节的尾部。它经常包含版权信息、法律信息链接和反馈建议用的地址。
    aside：定义和页面内容关联度较低的内容——如果被删除，剩下的内容仍然很合理。

### html5有哪些新特性

    a. HTML5 现在已经不是 SGML 的子集，主要是关于图像，位置，存储，多任务等功能的增加。
	b. 拖拽释放(Drag and drop) API
	c. 语义化更好的内容标签（header,nav,footer,aside,article,section）
	d. 音频、视频API(audio,video)
	e. 画布(Canvas) API
	f. 地理(Geolocation) API
	g. 本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失
	h. sessionStorage 的数据在页面会话结束时会被清除
	i. 表单控件，calendar、date、time、email、url、search 
	j. 新的技术webworker, websocket等

### HTML5引入什么新的表单属性？

    Datalist   datetime   output   keygen  date  month  week  time  number   range   emailurl

### HTML5废弃了哪些HTML4标签

    A.frame（框架）
    B.frameset（框架集）
    C.noframe（不支持框架的浏览器显示文本）
    D.applet（）
    E.big（大号字体）
    F.center（居中）
    G.basefront（默认字体颜色和字号）

### 哪些浏览器支持HTML5？

    几乎所有的浏览器Safari，Chrome，Firefox，Opera，IE9以上都支持HTML5

### HTML5的页面结构同HTML4或者更前的HTML有什么区别？

    一个典型的WEB页面包含头部，脚部，导航，中心区域，侧边栏。现在如果我们想在在HTML4的HTML区域中呈现这些内容，我们可能要使用DIV标签。
    但是在HTML5中通过为这些区域创建元素名称使他们更加清晰，也使得你的HTML更加可读
    <header>：代表HTML的头部数据
    <footer>：页面的脚部区域
    <nav>：页面导航元素
    <article>：自包含的内容
    <section>：使用内部article去定义区域或者把分组内容放到区域里
    <aside>：代表页面的侧边栏内容

### 除了audio和video，HTML5还有哪些媒体标签？

    <embed> 标签定义嵌入的内容，比如插件。
	<source> 对于定义多个数据源很有用。
	<track> 标签为诸如 video 元素之类的媒介规定外部文本轨道。 
	用于规定字幕文件或其他包含文本的文件，当媒介播放时，这些文件是可见的。

### 什么是响应式布局

    响应式布局是Ethan Marcotte在2010年5月份提出的一个概念，简而言之，就是一个网站能够兼容多个终端——而不是为每个终端做一个特定的版本。这个概念是为解决移动互联网浏览而诞生的。
    响应式布局可以为不同终端的用户提供更加舒适的界面和更好的用户体验，而且随着目前大屏幕移动设备的普及，用“大势所趋”来形容也不为过。随着越来越多的设计师采用这个技术，不仅看到很多的创新，还看到了一些成形的模式。

### 响应式布局该怎么设计

    1、 如何解决不同设备间的兼容问题?
		CSS3中的Media Query(媒介查询)可以解决这个问题。
	2、media query能够获取哪些值?
		设备的宽和高device-width，device-heigth显示屏幕/触觉设备。
		渲染窗口的宽和高width，heigth显示屏幕/触觉设备。
		设备的手持方向，横向还是竖向orientation(portrait|lanscape)和打印机等。
		画面比例aspect-ratio点阵打印机等。
		设备比例device-aspect-ratio-点阵打印机等。
		对象颜色或颜色列表color，color-index显示屏幕。
		设备的分辨率resolution
	3、语法结构及用法
		语法：@media 设备名 only (选取条件) not (选取条件) and(设备选取条件)，设备二{sRules}
	    用法：
		a、示例一：在link中使用@media：上面使用中only可省略，限定于计算机显示器，第一个条件max-width是指渲染界面最大宽度，第二个条件max-device-width是指设备最大宽度。

### 响应式布局有哪些优点和缺点

	优点：
		面对不同分辨率设备灵活性强
		能够快捷解决多设备显示适应问题
	缺点：
		兼容各种设备工作量大，效率低下
		代码累赘，会出现隐藏无用的元素，加载时间加长
		其实这是一种折中性质的设计解决方案，多方面因素影响而达不到最佳效果
		一定程度上改变了网站原有的布局结构，会出现用户混淆的情况

### 请解释一下CSS3的Flexbox（弹性盒布局模型），以及适用场景？

    一个用于页面布局的全新CSS3功能，Flexbox可以把列表放在同一个方向（从上到下排列，从左到右），并让列表能延伸到占用可用的空间。
    较为复杂的布局还可以通过嵌套一个伸缩容器（flex container）来实现。
    采用Flex布局的元素，称为Flex容器（flex container），简称"容器"。
    它的所有子元素自动成为容器成员，称为Flex项目（flex item），简称"项目"。
    常规布局是基于块和内联流方向，而Flex布局是基于flex-flow流可以很方便的用来做局中，能对不同屏幕大小自适应。
    在布局上有了比以前更加灵活的空间。

### 什么的媒体查询？

    媒体查询是向不同设备提供不同样式的一种不错方式，它为每种类型的用户提供了最佳的体验。作为CSS3规范的一部分，体查询扩展了media属性（控制您的样式应用方式）的角色。
    例如，多年来人们常常使用一种独立的样式表，通过指定media="print"来打印网页。媒体查询将这一理念提升到了更高层次，允许设计人员基于各种不同的设备属性（比如屏幕宽度、方向等）来确定目标样式。

### 常见媒体查询有哪些？

    如果目标是横向模式智能手机，则使用： @media (min-width: 321px) { ... }
    如果目标是纵向模式智能手机，则使用： @media (max-width: 320px) { ... }
    如果目标是横向模式 Apple iPad，则使用： @media (orientation: landscape) { ... }
    如果目标是纵向模式 iPad，则使用： @media (orientation: portrait) { ... }


### 如何编写媒体查询？

    要将媒体查询添加到media属性中，您可以使用表1中的媒体功能设置一个或多个条件。与CSS属性一样，在一个冒号后指定媒体功能的值。每个条件包含在圆括号中，使用关键字and添加到媒体声明中。
    例如：
        media="screen and (min-width: 401px) and (max-width: 600px)"

### 新的HTML5文档类型和字符集是？

    HTML5 文档类型很简单：<!doctype html>
	HTML5 使用 UTF-8 编码示例：<meta charset=”UTF-8″>

### HTML5中如何嵌入音频？

    HTML5 支持 MP3、Wav 和 Ogg 格式的音频，下面是在网页中嵌入音频的简单示
	<audio controls>
	    <source src=”jamshed.mp3″ type=”audio/mpeg”>
	    Your browser does’nt support audio embedding feature.
	</audio>

### HTML5的Canvas元素有什么用？

    Canvas 元素用于在网页上绘制图形，该元素标签强大之处在于可以直接在 HTML 上进行图形操作 其html语法如下
	<canvas id=”canvas1″ width=”300″ height=”100″></canvas>

### HTML5存储类型有什么区别？

    HTML5 能够本地存储数据，在之前都是使用 cookies 使用的。HTML5 提供了下面两种本地存储方案：
	localStorage 用于持久化的本地存储，数据永远不会过期，关闭浏览器也不会丢失。
	sessionStorage 同一个会话中的页面才能访问并且当会话结束后数据也随之销毁。
	因此sessionStorage不是一种持久化的本地存储，仅仅是会话级别的存储


### label标签的作用、应用

	1、lable标签主要是作为一种标题说明元素存储的，通常有：for关联、以及将form control放在label标签中的方式
	2、lable标签主要属性：
	   2.1、for属性，做标签关联，但for关联的必须是一个form control标签
	   2.2、accesskey属性：用于设置热键，但不能与浏览器热键冲突，否则会先触发浏览器的热键
	3、label的嵌套
	   3.1、labe标签内不能再嵌套label
	   3.2、label只能包含一个input子孙（包含checkbox、text等元素）、button、select、textarea元素
	   3.3、label嵌套时，事件的触发遵循冒泡原则
	4、for关联
       4.1、for关联，在labe标签上的事件，会触发关联元素的相应事件（并且关联元素的冒泡阻止动作无效）：
       		单击labeTow会做如下输出(label会先触发自身的事件，然后触发关联元素相应的事件)：
			labelTow…………….
			inputTow……………
			单击inpuTow会做如输出：
			inputTow………….
	5、label标签不能为a和button标签的后代
 	6、html5中对lable标签加了form属性，规则label所属的一个或多个表单


### 如何处理HTML5新标签的浏览器兼容问题？

    1. IE8/IE7/IE6支持通过 document.createElement 方法产生的标签，可以利用这一特性让这些浏览器支持 HTML5 新标签，浏览器支持新标签后，还需要添加标签默认的样式（当然最好的方式是直接使用成熟的框架、使用最多的是html5shim框架）


### 如何实现浏览器内多个标签页之间的通信

    WebSocket、SharedWorker；也可以调用localstorge、cookies等本地存储方式；
    localstorge另一个浏览上下文里被添加、修改或删除时，它都会触发一个事件，
    我们通过监听事件，控制它的值来进行页面信息通信；
    注意quirks：Safari 在无痕模式下设置localstorge值时会抛出 QuotaExceededError 的异常；

### HTML5应用程序缓存和浏览器缓存有什么区别

    应用程序缓存是 HTML5 的重要特性之一，提供了离线使用的功能，让应用程序可以获取本地的网站内容，
	例如 HTML、CSS、图片以及 JavaScript。这个特性可以提高网站性能，它的实现借助于 manifest 文件，与传统浏览器缓存相比，它不强制用户访问的网站内容被缓存。


### webSocket如何兼容低浏览器

    Adobe Flash Socket 、 ActiveX HTMLFile (IE) 、 基于 multipart 编码发送 XHR 、 基于长轮询的 XHR	

### HTML5的离线储存怎么使用，工作原理能不能解释一下？

    在用户没有与因特网连接时，可以正常访问站点或应用，在用户与因特网连接时，更新用户机器上的缓存文件。
    原理：HTML5的离线存储是基于一个新建的.appcache文件的缓存机制(不是存储技术)，通过这个文件上的解析清单离线存储资源，这些资源就会像cookie一样被存储了下来。之后当网络在处于离线状态下时，浏览器会通过被离线存储的数据进行页面展示。
    如何使用：
    1)页面头部像下面一样加入一个manifest的属性；
    2)在cache.manifest文件的编写离线存储的资源
    3)在离线状态时，操作window.applicationCache进行需求实现。

### 浏览器是怎么对HTML5的离线储存资源进行管理和加载的呢

    在线的情况下，浏览器发现html头部有manifest属性，它会请求manifest文件，如果是第一次访问app，那么浏览器就会根据manifest文件的内容下载相应的资源并且进行离线存储。如果已经访问过app并且资源已经离线存储了，那么浏览器就会使用离线的资源加载页面，然后浏览器会对比新的manifest文件与旧的manifest文件。
    如果文件没有发生改变，就不做任何操作，如果文件改变了，那么就会重新下载文件中的资源并进行离线存储。
    离线的情况下，浏览器就直接使用离线存储的资源。

### CSS3有哪些新特性？

    新增各种CSS选择器、CSS3实现圆角（border-radius），阴影（box-shadow），文字特效（text-shadow），文字渲染 （text-decoration），线性渐变（gradient），变形（transform） ，多背景 rgba，在CSS3中唯一引入的伪元素是::selection，媒体查询，多栏布局  

### CSS3的属性为什么要带前缀

    浏览器厂商以前就一直在实施CSS3，但它还未成为真正的标准。为此，当一些CSS3样式语法还存在波动时，它们提供针对浏览器的前缀。添加上私有前缀之后的CSS3属性可以说是对应浏览器的私有属性
    Webkit内核：前缀为-webkit
    Trident内核：前缀为-ms
    Gecko内核：前缀为-moz 
    Presto内核：前缀为-o 

### CSS3的rem单位与传统em的区别

    em是相对于其元素来设置字体大小的，这样就会存在一个问题，进行任何元素设置，都有可能需要知道他父元素的大小。
    而Rem是相对于根元素<html>，这个单位可谓集相对大小和绝对大小的优点于一身，通过它既可以做到只修改根元素就成比例地调整所有字体大小，又可以避免字体大小逐层复合的连锁反应。

### CSS3新增伪类有那些？

 	p:first-of-type 选择属于其父元素的首个 <p> 元素的每个 <p> 元素。
    p:last-of-type  选择属于其父元素的最后 <p> 元素的每个 <p> 元素。
    p:only-of-type  选择属于其父元素唯一的 <p> 元素的每个 <p> 元素。
    p:only-child        选择属于其父元素的唯一子元素的每个 <p> 元素。
    p:nth-child(n)  选择属于其父元素的第n个子元素的每个 <p> 元素。
    :after          在元素之前添加内容,也可以用来做清除浮动。
    :before         在元素之后添加内容
    :enabled        选择器匹配每个已启用的元素
    :disabled       控制表单控件的禁用状态。
    :checked        单选框或复选框被选中。

### before和after中双冒号和单冒号有什么区别？

    单冒号(:)用于CSS3伪类，双冒号(::)用于CSS3伪元素。（伪元素由双冒号和伪元素名称组成）
    双冒号是在当前规范中引入的，用于区分伪类和伪元素。不过浏览器需要同时支持旧的已经存在的伪元素写法。而新的在CSS3中引入的伪元素则不允许再支持旧的单冒号的写法。

---

##  JavaScript

### document。write和innerHTML的区别

    document.write
    a. 改变 HTML 输出流
    b. 当在文档加载之后使用 document.write()，这会覆盖该文档(即重绘整个页面)
    innerHTML
    a. 改变 HTML 内容（即重绘页面的一部分）

### javascript怎样添加、移除、移动、复制、创建节点

    createDocumentFragment()    //创建一个DOM片段
    createElement()   //创建一个具体的元素
    createTextNode()   //创建一个文本节点
    appendChild()      //添加
    removeChild()      //移除
    replaceChild()      //替换
    insertBefore()      //插入

### 简述列举文档对象模型DOM里document的常用的查找访问节点的方法

    Document.getElementById 根据元素id查找元素
    Document.getElementsByName 根据元素name查找元素
    Document.getElementsTagName 根据指定的元素名查找元素
    Document.querySelector 根据CSS选择器返回第一个查找元素。
    document.querySelectorAll根据CSS选择器返回所有查找元素。

### 请叙述下js的基本数据类型

    Undefined、Null、Boolean、Number、String、ES6 新增:Symbol（创建后独一无二且不可变的数据类型）

### 介绍js有哪些内置对象？

    Object 是 JavaScript 中所有对象的父对象
    数据封装类对象：Object、Array、Boolean、Number 和 String
    其他对象：Function、Arguments、Math、Date、RegExp、Error

### 什么是window对象什么是document对象

    简单来说，document是window的一个对象属性。
    Window 对象表示浏览器中打开的窗口。
    如果文档包含框架（frame 或 iframe 标签），浏览器会为 HTML 文档创建一个 window 对象，并为每个框架创建一个额的 window 对象。
    所有的全局函数和对象都属于Window 对象的属性和方法。
    document   对 Document 对象的只读引用。

### 列举浏览器对象模型BOM里常用的至少4个对象，并列举window对象的常用方法至少5个

    对象：window document location screen history navigator
    方法：alert() confirm() prompt() open() close()

### BOM对象有哪些，列举window对象？

    window对象 ，是JS的最顶层对象，其他的BOM对象都是window对象的属性；
    document对象，文档对象；
    location对象，浏览器当前URL信息；
    navigator对象，浏览器本身信息；
    screen对象，客户端屏幕信息；
    history对象，浏览器访问历史信息；

### 谈谈对this指针的理解，可以列举几种使用情况？

    a. 纯粹的函数调用，属于全局性调用，因此this就代表全局对象Global。
    b. 作为对象方法的调用，这时this就指这个上级对象。
    c. 作为构造函数调用，就是通过这个函数new一个新对象（object）。这时，this就指这个新对象。
    d. apply与call的调用，它们的作用是改变函数的调用对象，它的第一个参数就表示改变后的调用这个函数的对象。

### null和undefined的区别？

    null        表示一个对象是“没有值”的值，也就是值为“空”；
    undefined   表示一个变量声明了没有初始化(赋值)；
    undefined不是一个有效的JSON，而null是；
    undefined的类型(typeof)是undefined；

### 阐述下==和===的区别

    前者是判断值是否相等,而后者是判断值及类型是否完全相等。

### 面向对象的理解？

    面向对象就是在程序中，用一个对象描述现实中一个事物。为什么使用面向对象？因为面向对象更接近于人的思维方式，更便于代码维护。

### 面向对象的三大特点是什么？

    面向对象三大特点：封装，继承，多态 .
    封装：讲现实中一个事物的属性和方法，集中定义在程序中的一个对象中。为什么要封装：更接近于人的想法，便于代码维护。
    继承：父对象中的成员，子对象可以直接使用。为什么要继承：代码重用！节约内存空间
    多态：同一样东西，在不同情况下表现出不同的状态。


### new操作符具体干了什么呢

    a. 一个新对象被创建。它继承自函数原型
    b. 构造函数被执行。执行的时候，相应的传参会被传入
    c. 上下文(this)会被指定为这个新实例
    d. 如果构造函数返回了一个“对象”，那么这个对象会取代整个new出来的结果

### 请解释一下JavaScript的同源策略

    同源策略是浏览器有一个很重要的概念。所谓同源是指，域名，协议，端口相同。不同源的客户端脚本

    (javascript、ActionScript)在没明确授权的情况下，不能读写对方的资源。简单的来说，浏览器允许

    包含在页面A的脚本访问第二个页面B的数据资源，这一切是建立在A和B页面是同源的基础上。

### 如何解决跨域问题

    a. JSONP，填充式JSON（ 利用script标签的跨域能力 ）
    b. iframe跨域
    c. HTML5的window.postMessage方法跨域 
    d. 通过设置img的src属性，进行跨域请求
    e. 跨域资源共享（CORS），服务器设置Access-Control-Allow-OriginHTTP响应头之后，浏览器将会允许跨域请求

### eval是做什么的？

    a. eval()函数可计算某个字符串，并执行其中的的 JavaScript 代码。
    b. eval()是一个顶级函数并且跟任何对象无关。
    c. 如果字符串表示了一个表达式，eval()会对表达式求值。如果参数表示了一个或多个JavaScript声明， 那么eval()会执行声明。

### 已知ID的Input输入框，希望获取这个输入框的输入值，怎么做？

    document.getElementById(“ID”).value

### javascript函数有重载这个概念呢？

    定义JavaScript函数时，函数名是函数对象的标识，参数数量只是这个函数的属性。靠定义参数数量不同的函数实现重载是不行的。
    调用函数时，js通过函数名找到对应的函数对象，然后根据函数按照定义时的参数，和表达式参数列表
    按顺序匹配，多余的参数舍去，不够的参数按undefined处理，然后执行函数代码。所以，js重载函数需要通过函数代码判断参数值和类型实现。
    通常定义函数时，把必选参数放在参数列表最前面，可选参数放在参数放在参数列表必须参数后面，方便函数重载。

### 如何判断一个js对象是否是Array，最准确的方法是

    Object.prototype.toString.call(arr) === '[object Array]'; arr为待检测对象

### javascript的typeof返回哪些数据类型

    Object（array、Object） number function boolean underfind

### js如何获得一个DOM元素的绝对位置

    offsetTop：返回当前元素相对于其 offsetParent 元素的顶部的距离
    offsetLeft：返回当前元素相对于其 offsetParent 元素的左边的距离
    getBoundingClientRect()：返回值是一个DOMRect对象，它包含了一组用于描述边框的只读属性―left、top、right和bottom，属性单位为像素

### 同步和异步的区别

    同步是阻塞模式，异步是非阻塞模式。
    同步就是指一个进程在执行某个请求的时候，若该请求需要一段时间才能返回信息，那么这个进程将会一直等待下去，直到收到返回信息才继续执行下去；
    异步是指进程不需要一直等下去，而是继续执行下面的操作，不管其他进程的状态。当有消息返回时系统会通知进程进行处理，这样可以提高执行的效率。

### 谈谈JavaScript的作用域和作用域链

    JavaScript的作用域指的是变量的作用范围，内部作用域由函数的形参，实参，局部变量，函数构成，内部作用域和外部的作用域一层层的链接起来形成作用域链，当在在函数内部要访问一个变量的时候，首先查找自己的内部作用域有没有这个变量，如果没有就到这个对象的原型对象中去查找，还是没有的话，就到该作用域所在的作用域中找，直到到window所在的作用域，每个函数在声明的时候就默认有一个外部作用域的存在了。

### 什么是usestrict使用它区别是什么？

    ECMAscript 5添加了第二种运行模式："严格模式"（strict mode）这种模式使得 Javascript 在更严格的条件下运行
    设立"严格模式"的目的，主要有以下几个：
    a. 消除Javascript语法的一些不合理、不严谨之处，减少一些怪异行为;
    b. 消除代码运行的一些不安全之处，保证代码运行的安全；
    c. 提高编译器效率，增加运行速度；
    d. 为未来新版本的Javascript做好铺垫。

### call和apply的区别是什么？

    call 和 apply 就是为了改变函数体内部 this 的指向。
    区别是从第二个参数起，call 需要把参数按顺序传递进去，而 apply 则是把参数放在数组里。

### 在Javascript中什么是伪数组？如何将伪数组转化为标准数组？

    伪数组（类数组）：无法直接调用数组方法或期望length属性有什么特殊的行为，但仍可以对真正数组
    遍历方法来遍历它们。典型的是函数的argument参数，还有像调用
    getElementsByTagName,document.childNodes之类的，它们都返回NodeList对象都属于伪数组。可以使用Array.prototype.slice.call(fakeArray)将数组转化为真正的Array对象。

### Javascript中callee和caller的作用？

    caller是返回一个对函数的引用，该函数调用了当前函数；
    callee是返回正在被执行的function函数，也就是所指定的function对象的正文

### JavaScript中的变量声明提升？

函数声明和变量声明总是被JavaScript解释器隐式地提升到包含他们的作用域的最顶端。
函数表达式中只会提升名称，函数体只有在执行到赋值语句时才会被赋值。

### 请解释一下什么是闭包

    闭包是一种特殊的对象。它由两部分构成：函数，以及创建该函数的环境。
    可以把闭包简单理解成 "定义在一个函数内部的函数"，闭包就是将函数内部和函数外部连接起来的一座桥梁。
    闭包有如下特性：
    a. JavaScript允许你使用在当前函数以外定义的变量
    b. 即使外部函数已经返回，当前函数仍然可以引用在外部函数所定义的变量
    c. 闭包可以更新外部变量的值
    d. 用闭包模拟私有方法
    由于闭包会使得函数中的变量都被保存在内存中，内存消耗很大，所以不能滥用闭包，否则会造成网页的性能问题

### 解释下JavaScript原型，原型链

    原型：
    a. 原型是一个对象，其他对象可以通过它实现属性继承。
    b. 一个对象的真正原型是被对象内部的[[Prototype]]属性(property)所持有。浏览器支持非标准的访问器__proto__。
    c. 在javascript中，一个对象就是任何无序键值对的集合，如果它不是一个主数据类型(undefined，null，boolean，number，string)，那它就是一个对象。
    原型链：
    a. 因为每个对象和原型都有一个原型(注:原型也是一个对象)，对象的原型指向对象的父，而父的原型又指向父的父，我们把这种通过原型层层连接起来的关系撑为原型链。
    b. 这条链的末端一般总是默认的对象原型。

### 描述一下cookies，sessionStorage和localStorage的区别

    sessionStorage用于本地存储一个会话（session）中的数据，这些数据只有在同一个会话中的页面才能访问并且当会话结束后数据也随之销毁。因此sessionStorage不是一种持久化的本地存储，仅仅是会话级别的存储。而localStorage用于持久化的本地存储，除非主动删除数据，否则数据是永远不会过期的。
    web storage和cookie的区别
    Web Storage的概念和cookie相似，区别是它是为了更大容量存储设计的。Cookie的大小是受限的，并且
    每次你请求一个新的页面的时候Cookie都会被发送过去，这样无形中浪费了带宽，另外cookie还需要指定作用域，不可以跨域调用。除此之外，Web Storage拥有setItem,getItem,removeItem,clear等方法，不像cookie需要前端开发者自己封装setCookie，getCookie。但是Cookie也是不可以或缺的：Cookie的作用是与服务器进行交互，作为HTTP规范的一部分而存在 ，而Web Storage仅仅是为了在本地“存储”数据而生。


### 什么是Cookie隔离？

    如果静态文件都放在主域名下，那静态文件请求的时候都带有的cookie的数据提交给server的，非常浪费流量，所以不如隔离开。
    因为cookie有域的限制，因此不能跨域提交请求，故使用非主要域名的时候，请求头中就不会带有cookie数据，这样可以降低请求头的大小，降低请求时间，从而达到降低整体请求延时的目的。同时这种方式不会将cookie传入Web Server，也减少了Web Server对cookie的处理分析环节，提高了webserver的http请求的解析速度。

### 在JavaScript中，常用的绑定事件的方法有哪些？

    a. 在DOM元素中直接绑定，DOM元素，可以理解为HTML标签，onXXX="JavaScript Code"
    b. 在JavaScript代码中绑定，elementObject.onXXX=function(){}，通称为DOM0事件系统。
    c. 绑定事件监听函数，标准浏览器使用 addEventListener() ，IE11以下版本attachEvent() 来绑定事件监听函数，通称为DOM2事件系统。

### 请解释什么是事件代理

    事件代理（Event Delegation），又称之为事件委托。是 JavaScript 中常用绑定事件的常用技巧。顾名思义，“事件代理”即是把原本需要绑定的事件委托给父元素，让父元素担当事件监听的职务。事件代理的原理是DOM元素的事件冒泡。使用事件代理的好处是可以提高性能。

### javascript的事件流模型都有什么？

    “事件冒泡”：事件开始由最具体的元素接受，然后逐级向上传播
    “事件捕捉”：事件由最不具体的节点先接收，然后逐级向下，一直到最具体的
    “DOM事件流”：三个阶段：事件捕捉，目标阶段，事件冒泡

### 事件是？IE与火狐的事件机制有什么区别？如何阻止冒泡？

    a. 我们在网页中的某个操作（有的操作对应多个事件）。例如：当我们点击一个按钮就会产生一个事件。是可以被 JavaScript 侦测到的行为。
    b. 事件处理机制：IE是事件冒泡、Firefox同时支持两种事件模型，也就是：捕获型事件和冒泡型事件；
    c. ev.stopPropagation();（旧ie的方法 ev.cancelBubble = true;）

### 谈谈对JSON的理解

    JSON(JavaScript Object Notation) 是一种轻量级的数据交换格式。
    它是基于JavaScript的一个子集。数据格式简单, 易于读写, 占用带宽小
    如：{"age":"12", "name":"back"}

### 请你谈谈Cookie的弊端

    a. 每个特定的域名下最多生成的cookie个数有限制
    b. IE和Opera 会清理近期最少使用的cookie，Firefox会随机清理cookie
    c. cookie的最大大约为4096字节，为了兼容性，一般不能超过4095字节
    d. 安全性问题。如果cookie被人拦截了，那人就可以取得所有的session信息。 

### Ajax读取一个XML文档并进行解析的实例

    a. 初始化一个HTTP请求，IE以ActiveX对象引入。后来标准浏览器提供了XMLHttpRequest类，它支持ActiveX对象所提供的方法和属性
    b. 发送请求，可以调用HTTP请求类的open()和send()方法
    c. 处理服务器的响应，通过http_request.onreadystatechange = nameOfTheFunction。来指定函数

### ajax的readystate有5个状态，每个状态表示什么？

    0 － （未初始化）还没有调用send()方法 
    1 － （载入）已调用send()方法，正在发送请求 
    2 － （载入完成）send()方法执行完成，已经接收到全部响应内容 
    3 － （交互）正在解析响应内容 
    4 － （完成）响应内容解析完成，可以在客户端调用了 

### Ajax有哪些好处和弊端？

    优点：
    a. 无刷新更新数据
    b. 异步与服务器通信
    c. 前端和后端负载平衡
    d. 基于标准被广泛支持
    e. 界面与应用分离
    缺点：
    a. AJAX干掉了Back和History功能，即对浏览器机制的破坏
    b. AJAX的安全问题
    c. 对搜索引擎支持较弱
    d. 违背URL和资源定位的初衷

### AJAX应用和传统Web应用有什么不同

    在传统的Javascript编程中，如果想得到服务器端数据库或文件上的信息，或者发送客户端信息到服务器，需要建立一个HTML form然后GET或者POST数据到服务器端。用户需要点击”Submit”按钮来发送或者接受数据信息，然后等待服务器响应请求，页面重新加载。
    因为服务器每次都会返回一个新的页面， 所以传统的web应用有可能很慢而且用户交互不友好。使用AJAX技术， 就可以使Javascript通过XMLHttpRequest对象直接与服务器进行交互。
    通过HTTP Request， 一个web页面可以发送一个请求到web服务器并且接受web服务器返回的信息(不用重新加载页面)，展示给用户的还是通一个页面，用户感觉页面刷新，也看不到到Javascript后台进行的发送请求和接受响应。

### Flash、Ajax各自的优缺点，在使用中如何取舍？

    Flash适合处理多媒体、矢量图形、访问机器，但对CSS、处理文本上不足，不容易被搜索
    Ajax对CSS、文本支持很好，支持搜索，但多媒体、矢量图形、机器访问不足
    共同点：与服务器的无刷新传递消息、可以检测用户离线和在线状态、操作DOM

### GET和POST的区别，何时使用POST？

    GET：一般用于信息获取，使用URL传递参数，对所发送信息的数量也有限制，一般在2000个字符
    POST：一般用于修改服务器上的资源，对所发送的信息没有限制
    GET方式需要使用 Request.QueryString 来取得变量的值
    POST方式通过 Request.Form 来获取变量的值
    也就是说 Get 是通过地址栏来传值，而 Post 是通过提交表单来传值。
    在以下情况中，请使用 POST 请求：
    a. 无法使用缓存文件（更新服务器上的文件或数据库）
    b. 向服务器发送大量数据（POST 没有数据量限制）
    c. 发送包含未知字符的用户输入时，POST 比 GET 更稳定也更可靠

### 如何判断当前脚本运行在浏览器还是node环境中？

    通过判断Global对象是否为window，如果是window，当前脚本运行在浏览器中

### JS模块的封装方法，比如怎样实现私有变量，不能直接赋值，只能通过公有方法

    a. 通过json生成对象的原始模式，多写几个就会非常麻烦，也不能反映出它们是同一个原型对象的实例
    b. 原始模式的改进，可以写一个函数，解决代码重复的问题。同样不能反映出它们是同一个原型对象的
    实例
    c. 构造函数模式，就是一个普通函数，不过内部使用了this变量，但是存在一个浪费内存的问题。
    d. Prototype模式，每一个构造函数都有一个prototype属性，指向另一个对象。这个对象的所有属性和
    方法，都会被构造函数的实例继承，可以把那些不变的属性和方法，直接定义在prototype对象上。 
    Prototype模式的验证方法：：isPrototypeOf()、hasOwnProperty()和in运算符。


### JavaScript的值类型和引用类型

    JavaScript有两种类型的数据，值类型和引用类型，一般的数字，字符串，布尔值都是值类型，存放在栈中，而对象，函数，数组等是引用类型，存放在堆中，对引用类型的复制其实是引用复制，相当于复制着地址，对象并没有真正的复制。    

### 阐述下split与join的区别

    join函数获取一批字符串，然后用分隔符字符串将它们连接起来，从而返回一个字符串。  
    split()函数获取一个字符串，然后在分隔符处将其断开，从而返回一批字符串。
    但是，这两个函数之间的区别在于join可以使用任何分割字符串将多个字符串连接起来，而split()只能使用一个字符分隔符将字符串断开。

### JavaScript中，有一个函数，执行时对象查找时，永远不会去查找原型，这个函数是？

    hasOwnProperty 
    用法：object.hasOwnProperty(proName)
    其中参数object是必选项。一个对象的实例。
    proName是必选项。一个属性名称的字符串值。


### 阐述下什么是块级作用域

    任何一对花括号（｛和｝）中的语句集都属于一个块，在这之中定义的所有变量在代码块外都是不可见的，我们称之为块级作用域。

### HTTP状态消息200、302、304、403、404、500分别表示什么

    200：请求已成功，请求所希望的响应头或数据体将随此响应返回。
    302：请求的资源临时从不同的 URI响应请求。由于这样的重定向是临时的，客户端应当继续向原有地址发送以后的请求。只有在Cache-Control或Expires中进行了指定的情况下，这个响应才是可缓存的
    304：如果客户端发送了一个带条件的 GET 请求且该请求已被允许，而文档的内容（自上次访问以来或者根据请求的条件）并没有改变，则服务器应当返回这个状态码。304响应禁止包含消息体，因此始终以消息头后的第一个空行结尾。
    403：服务器已经理解请求，但是拒绝执行它。
    404：请求失败，请求所希望得到的资源未被在服务器上发现。
    500：服务器遇到了一个未曾预料的状况，导致了它无法完成对请求的处理。一般来说，这个问题都会在服务器端的源代码出现错误时出现。


### js延迟加载的方式有哪些？

    a. 将script节点放置在最后之前
    b. 使用script标签的defer和async属性，defer属性为延迟加载，是在页面渲染完成之后再进行加载的，而async属性则是和文档并行加载
    c. 通过监听onload事件，动态添加script节点
    d. 通过ajax下载js脚本，动态添加script节点

### requireJS的核心原理是什么？

    核心是js的加载模块，通过正则匹配模块以及模块的依赖关系，保证文件加载的先后顺序，根据文件的路径对加载过的文件做了缓存

### 内存泄露是什么，哪些操作会造成内存泄漏？

    内存泄漏指任何对象在您不再拥有或需要它之后仍然存在。
    垃圾回收器定期扫描对象，并计算引用了每个对象的其他对象的数量。如果一个对象的引用数量为 0（没有其他对象引用过该对象），或对该对象的惟一引用是循环的，那么该对象的内存即可回收。
    a. setTimeout 的第一个参数使用字符串而非函数的话，会引发内存泄漏。
    b. 闭包
    c. 控制台日志
    d. 循环（在两个对象彼此引用且彼此保留时，就会产生一个循环）

### AMD、CMD规范区别？

    两者都是异步模块定义的一个实现；CMD和AMD都是CommonJS的一种规范的实现定义，RequireJS和SeaJS是对应的实践；
    CMD和AMD的区别：CMD相当与按需加载，定义一个模块的时候不需要立即制定依赖模块，在需要的时候require就可以了，比较方便；而AMD则相反，定义模块的时候需要制定依赖模块，并以形参的方式引入factory中。

### 如何在页面上实现一个圆形的可点击区域？

    1)map+area或者svg
    2)border-radius 
    3)纯js实现 需要求一个点在不在圆上简单算法、获取鼠标坐标等等

### 谈谈对ES6相对ES5增加了哪些扩展

    新增模板字符串（为JavaScript提供了简单的字符串插值功能）、箭头函数（操作符左边为输入的参数，而右边则是进行的操作以及返回的值Inputs=>outputs。）、for-of（用来遍历数据—例如数组中的值。）arguments对象可被不定参数和默认参数完美代替。
    ES6将promise对象纳入规范，提供了原生的Promise对象。增加了let和const命令，用来声明变量。增加了块级作用域。let命令实际上就增加了块级作用域。
    ES6规定，var命令和function命令声明的全局变量，属于全局对象的属性；let命令、const命令、class命令声明的全局变量，不属于全局对象的属性。。还有就是引入module模块的概念

### ECMAScript和JavaScript的关系

    ECMAScript和JavaScript的关系是，前者是后者的规格，后者是前者的一种实现（另外的ECMAScript方言还有Jscript和ActionScript）。日常场合，这两个词是可以互换的。


### ECMAScript6怎么写class，为什么会出现class这种东西

    class method{ }; 通过class关键字，可以定义类。基本上，ES6的class可以看作只是一个语法糖，它的绝大部分功能，ES5都可以做到，新的class写法只是让对象原型的写法更加清晰、更像面向对象编程的语法而已。  

### ECMAScript6引入了let它与传统的var有何区别？

    同是用来声明变量。它的用法类似于var，但是所声明的变量，只在let命令所在的代码块内有效。
    区别：let不像var那样会发生“变量提升”现象。
    let不允许在相同作用域内，重复声明同一个变量。
    let 允许把变量的作用域限制在块级域中。与 var 不同处是：var 申明变量要么是全局的，要么是函数级的，而无法是块级的。

### 谈谈对ES6const的理解

    const声明一个只读的常量。一旦声明，常量的值就不能改变。它与let类似不可重复声明，不能变量提升，也具有块级作用域。

### ES6比较操作符

    两等号判等，会在比较时进行类型转换；三等号判等(判断严格)，比较时不进行隐式类型转换,（类型不同则会返回false）； 
    Object.is 在三等号判等的基础上特别处理了 NaN 、-0 和 +0 ，保证 -0 和 +0 不再相同，
    但 Object.is(NaN, NaN) 会返回 true.
    Object.is 应被认为有其特殊的用途，而不能用它认为它比其它的相等对比更宽松或严格。

---

##  jQuery

### 什么是jQuery？
    jQuery是一个快速、简洁的JavaScript框架，是继Prototype之后又一个优秀的JavaScript代码库（或JavaScript框架）。jQuery设计的宗旨是“write Less，Do More”，即倡导写更少的代码，做更多的事情。
    它封装JavaScript常用的功能代码，提供一种简便的JavaScript设计模式，优化HTML文档操作、事件处理、动画设计和Ajax交互

### body中的onload函数和jQuery中jquerydocument。ready有什么区别？

    a.我们可以在页面中使用多个$(document).ready()，但只能使用一次onload()。
    b. $(document).ready()函数在页面DOM元素加载完以后就会被调用，而onload()函数则要在所有的关联资源（包括图像、音频）加载完毕后才会调用。

### 阐述下jquery。extend与jquery。fn。extend的区别？

    jquery.extend 为jquery类添加类方法，可以理解为添加静态方法
    源码中jquery.fn = jquery.prototype，所以对jquery.fn的扩展，就是为jquery类添加成员函数
    使用：jquery.extend扩展，需要通过jquery类来调用，而jquery.fn.extend扩展，所有jquery实例都可以直接调用。

### 阐述下bind，live，delegate的区别

    bind： 绑定事件，对新添加的事件不起作用，方法用于将一个处理程序附加到每个匹配元素的事件上并返回jQuery对象。
    live： 方法将一个事件处理程序附加到与当前选择器匹配的所有元素（包含现有的或将来添加的）的指定事件上并返回jQuery对象。
    delegate： 方法基于一组特定的根元素将处理程序附加到匹配选择器的所有元素（现有的或将来的）的一个或多个事件上。

### 怎样才能jQuery对象与DOM对象之间的转换

    jquery转DOM对象:jQuery 对象是一个数组对象，可以通过[index]的丰富得到相应的DOM对象还可以通过get[index]去得到相应的DOM对象。
    DOM对象转jQuery对象:$(DOM对象)

### $(this)和this关键字在jQuery中有何不同？

    $(this) 返回一个 jQuery 对象，你可以对它调用多个 jQuery 方法，比如用 text() 获取文本，用val() 获取值等等。
    而 this 代表当前元素，它是 JavaScript 关键词中的一个，表示上下文中的当前 DOM 元素。

### jquery中get（）提交和post（）提交有区别吗？

    a .$.get() 方法使用GET方法来进行异步请求的。$.post() 方法使用POST方法来进行异步请求的。
    b .get请求会将参数跟在URL后进行传递，而POST请求则是作为HTTP消息的实体内容发送给Web服务器的，这种传递是对用户不可见的。
    c .get方式传输的数据大小不能超过2KB 而POST要大的多
    d .GET 方式请求的数据会被浏览器缓存起来，因此有安全问题。

### jquery和javascript有什么区别？

    JavaScript 是一种脚本语言，主要用在浏览器中，实现对网页的文档对象的操作和一些用户交互动作的处理。
    而 jQuery 则是 JavaScript 的一个代码库（或习惯性叫类库），它将一些在 JavaScript 开发中经常用到的功能集合起来，以方便开发者直接使用，而不需要再用原生 JavaScript 语句写大量代码，同时可在不同浏览器间实现一致的效果。

### jQuery与jQueryUI有啥区别？

    jQuery是一个js库，主要提供的功能是选择器，属性修改和事件绑定等等。
    jQuery UI则是在jQuery的基础上，利用jQuery的扩展性，设计的插件。提供了一些常用的界面元素，诸如对话框、拖动行为、改变大小行为等等

### jQuery中jquery（′class′）和jQuery中jquery('div.class')哪个效率更高？

    jQuery内部使用Sizzle引擎，处理各种选择器。Sizzle引擎的选择顺序是从右到左，所以这条语句是先选.class，
    第二个会直接过滤出div标签，而第一个就不会过滤了，将所有相关标签都列出。

### jQuery中detach（）和remove（）方法的区别是什么

    尽管 detach() 和 remove() 方法都被用来移除一个DOM元素, 两者之间的主要不同在于 detach() 会保
    持对过去被解除元素的跟踪, 因此它可以被取消解除, 而 remove() 方法则会保持过去被移除对象的引
    用. 

### jQuery的slideUp动画，如果目标元素是被外部事件驱动，当鼠标快速地连续触发外部元素事件，动画会滞后的反复执行，该如何处理呢

    stop() 方法停止当前正在运行的动画。
    jQuery stop(stopAll,goToEnd)方法: 如：$("#div").stop().slideUp();

### 在一个jQuery事件处理程序里返回了false会怎样？

    这通常用于阻止事件向上冒泡。

### 哪种方式更高效：document

    第一种，因为它直接调用了 JavaScript 引擎。

### 使用CDN加载jQuery库的主要优势是什么

    CDN的全称是Content Delivery Network，即内容分发网络
    CDN的基本原理是：广泛采用各种缓存服务器，将这些缓存服务器分布到用户访问相对集中的地区或者网络中，在用户访问网站时，利用全局负载技术将用户的访问指向距离最近的工作正常的缓存服务器上，由缓存服务器直接响应用户的请求。
    使用CDN加载jQuery一方面可以节省带宽，另一方面可以提高页面的加载速度同时也可以节省自己空间的
    流量

### 叙述下jQuery的特点

    a. 一款轻量级的js库
    b. 丰富快速的DOM选择器
    c. 链式表达式
    d. 事件、样式、动画等特效支持
    e. Ajax操作封装，支持跨域
    f. 跨浏览器兼容
    g. 插件扩展开发
