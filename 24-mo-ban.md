# 模板
模板主要包括三类：基于字符串的模板(String-based)、基于DOM的模板(DOM-based)、活动模板(Living Template)

##2.4.1 基于字符串的模板(String-based)

1、基于字符串的模板(String-based)，解决方案包括(dustjs、hogan.js、dot.js)
 
 ![](/assets/string-based.jpg)
 
 
**原理如下**：输入一段模板字符串，通过编译之后 ，生成一段Function，通过Function的render或类render函数渲染输入的数据data，输出模板字符串，字符串通过innerHTML或类似的方式渲染成最后的DOM结构。这类模板的问题在于通过字符串生成DOM之后就不再变化，如果在改变输入的数据data，需要重新render，重新生成一个全新的DOM结构，性能较差。但该模板可以在服务器端运行

![](/assets/string-based-template.png)


## 2.4.2 基于DOM的模板(DOM-based)

基于DOM的模板(DOM-based)，解决方案包括(angularjs、vuejs、knockout)

![](/assets/dom-based.jpg)
 
 
原理如下：将输入的字符串模板通过innerHTML转换为一个无状态DOM树，然后遍历该节点树，去抓取关键属性或语句，来进行相关的绑定，进而变成了有状态的DOM树，最终导致DOM树会与数据模型model进行绑定。这类模板的特点是修改数据时，会使有状态的DOM树实时更新，运行时性能更好，也会保留 DOM 中的已有事件


![](/assets/dom-based-template.png)


## 2.4.3 基于DOM的模板(DOM-based)

活动模板(Living Template)，解决方案包括(RegularJS、RactiveJS、htmlbar)

![](/assets/living-template.jpg)


原理如下：活动模板融合了字符串模板和DOM模板的技术，模板字符串string通过自定义的解析器DSL-based Parse解析成AST(抽象语法树)，通过遍历AST，使用createElement()、setAttribute()等原生DOM方法，生成DOM树，最终导致DOM树会与数据模型model进行绑定。由于其内部完全不使用innerHTML，所以安全性较高

![](/assets/living-template-engine.png)


