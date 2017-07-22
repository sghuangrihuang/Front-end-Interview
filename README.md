﻿#   前端面试题总结

##  一、WEB理论
* 各大浏览器的内核分别是什么?
* 介绍一下你对浏览器内核的理解？
* 前端页面有哪三层构成，分别是什么？作用是什么？
* 讲讲输入完网址按下回车，到看到网页这个过程中发生了什么
* 谈谈你对前端性能优化的理解
* 请说出三种减少页面加载时间的方法
* 列举IE与其他浏览器不一样的特性？
* 一个页面上有大量的图片（大型电商网站），加载很慢，你有哪些方法优化这些图片的加载，给用户更好的体验。
* 网站重构的理解
* 谈谈对“回流”的理解
* 线程与进程的区别
* 网页验证码是干嘛的，是为了解决什么安全问题。
* 什么是“前端路由”?什么时候适合使用“前端路由”? “前端路由”有哪些优点和缺点?
* 谈谈对前端模块化的理解
* 移动端的点击事件的有延迟，时间是多久，为什么会有？
* 你如何对网站的文件和资源进行优化?
* 请介绍一下渐进增强和优雅降级？
* 什么是盒子模型？
* 一个页面从输入 URL 到页面加载显示完成，这个过程中都发生了什么？（流程说的越详细越好）
* 是否了解公钥加密和私钥加密。

##  二、HTML+CSS
* 请解释一下什么是语义化的HTML。
* HTML与XHTML——二者有什么区别
* img标签上title属性与alt属性的区别是什么？
* 如果设计中使用了非标准的字体，你该如何去实现？
* 每个HTML文件里开头都有个很重要的东西，Doctype，知道这是干什么的吗？
* 你知道多少种Doctype文档类型？
* Doctype作用? 严格模式与混杂模式如何区分？它们有何意义?
* 简述一下src与href的区别
* 请阐述table的缺点
* 分别写出以下几个HTML标签：文字加粗、下标、居中、字体
* iframe的优缺点？
* 行内元素有哪些？块级元素有哪些？ 空(void)元素有那些？
* CSS中 link 和@import 的区别是什么？
* 对WEB标准以及W3C的理解与认识？
* 说下行内元素和块级元素的区别?行内块元素的兼容性使用?
* 为什么要初始化CSS样式？
* 有哪项方式可以对一个DOM设置它的CSS样式？
* 什么是 FOUC（无样式内容闪烁）？你如何来避免 FOUC？
* :link、:visited、:hover、:active的执行顺序是怎么样的？
* rgba()和opacity的透明效果有什么不同？
* display:none和visibility:hidden的区别？
* 对BFC规范的理解
* css的基本语句构成是?
* 请简述CSS的权重规则
* CSS优先级算法如何计算？
* css属性content有什么作用？有什么应用？
* line-height三种赋值方式有何区别？（带单位、纯数字、百分比）
* position包含几种属性？absolute和relative的区别？
* position的absolute与fixed共同点与不同点
* 请列举几种隐藏元素的方法
* css如何让一段文本中的所有英文单词的首字母大写
* 请列举几种可以清除浮动的方法
* 浏览器是怎样解析CSS选择器的？
* 请简述CSS样式表继承
* 在CSS样式中常使用px、em，各有什么优劣，在表现上有什么区别
* 什么是外边距重叠？重叠的结果是什么
* CSS 中类 (class) 和 ID 的区别。
* 请解释浮动 (Float) 及其工作原理。
* CSS伪类与CSS伪对象的区别
* 列出display的值，说明他们的作用
* box-sizing常用的属性有哪些?分别有什么作用? 
* css中可继承的属性有哪些？
* 如何解决img下的留白 ？
* 如何居中div？ 
* 什么是CSS Hack?
* 当float和margin同时使用时，IE6的双倍边距BUG如何解决?
* 请简述CSS的选择器
* 经常遇到的浏览器兼容性有哪些？
* 浮动元素引起的问题
* 如何使得文字不换行
* 用纯CSS创建一个三角形的原理是什么？
* 让页面里的字体变清晰，变细用CSS怎么做？
* 如何修改chrome记住密码后自动填充表单的黄色背景 ？
* font-style属性可以让它赋值为“oblique” oblique是什么意思？
* css多列等高如何实现？
* margin和padding分别适合什么场景使用？
* zoom:1的清除浮动原理?
* 请说出三种减低页面加载时间的方法
* 什么是CSS 预处理器 / 后处理器？
* 解释下 CSS sprites原理，优缺点
* Quirks模式是什么？它和Standards模式有什么区别？

##  三、HTML5+CSS3

* 什么是HTML5？
* HTML5 为什么只需要写 <!Doctype html>?
* 请写出至少5个html5新增的标签，并说明其语义和应用场景
* html5有哪些新特性
* HTML5 引入什么新的表单属性？
* HTML5 废弃了哪些 HTML4 标签
* 哪些浏览器支持HTML5？
* HTML5的页面结构同HTML4或者更前的HTML有什么区别？
* 除了 audio 和 video，HTML5 还有哪些媒体标签？
* 什么是响应式布局
* 响应式布局该怎么设计?
* 响应式布局有哪些优点和缺点?
* 请解释一下CSS3的Flexbox（弹性盒布局模型），以及适用场景？
* 什么的媒体查询？
* 常见媒体查询有哪些？
* 如何编写媒体查询？
* 新的 HTML5 文档类型和字符集是？
* HTML5 中如何嵌入音频？
* HTML5 Canvas 元素有什么用？
* HTML5 存储类型有什么区别？
* label标签的作用、应用
* 如何处理HTML5新标签的浏览器兼容问题？
* 如何实现浏览器内多个标签页之间的通信?
* HTML5 应用程序缓存和浏览器缓存有什么区别
* webSocket如何兼容低浏览器
* HTML5的离线储存怎么使用，工作原理能不能解释一下？
* 浏览器是怎么对HTML5的离线储存资源进行管理和加载的呢
* CSS3有哪些新特性？
* CSS3的属性为什么要带前缀
* CSS3的rem单位与传统em的区别
* CSS3新增伪类有那些？
* ::before 和 :after中双冒号和单冒号 有什么区别？
##  四、JavaScript
* document.write和 innerHTML的区别
* javascript怎样添加、移除、移动、复制、创建节点
* 简述列举文档对象模型DOM里document的常用的查找访问节点的方法
* 请叙述下js的基本数据类型
* 介绍js有哪些内置对象？
* 什么是window对象? 什么是document对象?
* 列举浏览器对象模型BOM里常用的至少4个对象，并列举window对象的常用方法至少5个
* BOM对象有哪些，列举window对象？
* 谈谈对this指针的理解，可以列举几种使用情况？
* null和undefined的区别？
* 阐述下“==”和“===”的区别 .
* 面向对象的理解 ？
* 面向对象的三大特点是什么？
* new操作符具体干了什么呢?
* 请解释一下 JavaScript 的同源策略
* 如何解决跨域问题?
* eval是做什么的？
* 已知ID的Input输入框，希望获取这个输入框的输入值，怎么做？
* javascript函数有重载这个概念呢？
* 如何判断一个js对象是否是Array，最准确的方法是
* javascript的typeof返回哪些数据类型
* js如何获得一个DOM元素的绝对位置
* 同步和异步的区别?
* 谈谈JavaScript的作用域和作用域链
* 什么是 "use strict" ?使用它区别是什么？
* call 和 apply 的区别是什么？
* 在Javascript中什么是伪数组？如何将伪数组转化为标准数组？
* Javascript中callee和caller的作用？
* JavaScript中的变量声明提升？
* 请解释一下什么是闭包
* 解释下JavaScript原型，原型链?
* 描述一下cookies，sessionStorage和localStorage的区别
* 什么是Cookie 隔离？
* 在JavaScript中，常用的绑定事件的方法有哪些？
* 请解释什么是事件代理
* javascript的事件流模型都有什么？
* 事件是？IE与火狐的事件机制有什么区别？ 如何阻止冒泡？
* 谈谈对JSON的理解
* 请你谈谈Cookie的弊端
* Ajax读取一个XML文档并进行解析的实例
* ajax的readystate有5个状态 ，每个状态表示什么？
* Ajax有哪些好处和弊端？
* AJAX应用和传统Web应用有什么不同
* Flash、Ajax各自的优缺点，在使用中如何取舍？
* GET和POST的区别，何时使用POST？
* 如何判断当前脚本运行在浏览器还是node环境中？
* JS模块的封装方法，比如怎样实现私有变量，不能直接赋值，只能通过公有方法
* JavaScript的值类型和引用类型
* 阐述下split() 与join() 的区别
* JavaScript中，有一个函数，执行时对象查找时，永远不会去查找原型，这个函数是？
* 阐述下什么是块级作用域
* HTTP状态消息200 302 304 403 404 500分别表示什么
* js延迟加载的方式有哪些？
* requireJS的核心原理是什么？
* 内存泄露是什么，哪些操作会造成内存泄漏？
* AMD、CMD规范区别？
* 如何在页面上实现一个圆形的可点击区域？
* 谈谈对ES6相对ES5 增加了哪些扩展
* ECMAScript和JavaScript的关系
* ECMAScript6 怎么写class，为什么会出现class这种东西?
* ECMAScript6 引入了let 它与传统的var 有何区别？
* 谈谈对ES6 const的理解
* ES6中Object.is() 与原来的比较操作符“ ===”、“ ==”的区别？
##  五、jQuery
* 什么是jQuery？
* body中的onload()函数和jQuery中的$(document).ready()有什么区别？
* 阐述下jquery.extend 与 jquery.fn.extend的区别？
* 阐述下bind(), live(), delegate()的区别
* 怎样才能jQuery对象与DOM对象之间的转换
* $(this) 和 this 关键字在 jQuery 中有何不同？
* jQuery 中的方法链是什么？使用方法链有什么好处？
* jquery中$.get()提交和$.post()提交有区别吗？
* jquery和javascript有什么区别？
* jQuery与jQuery UI 有啥区别？
* jQuery中 $(′.class′)和$('div.class') 哪个效率更高？
* jQuery中 detach() 和 remove() 方法的区别是什么? 
* jQuery 的 slideUp动画 ，如果目标元素是被外部事件驱动, 当鼠标快速地连续触发外部元素事件, 动画会滞后的反复执行，该如何处理呢?
* 在一个 jQuery 事件处理程序里返回了 false 会怎样？
* 哪种方式更高效：document.getElementbyId(“myId”) 还是 $(“#myId”)？
* 使用 CDN 加载 jQuery 库的主要优势是什么 ? 
* 叙述下jQuery的特点
