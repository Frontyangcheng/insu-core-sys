# 模板
模板主要包括三类：基于字符串的模板(String-based)、基于DOM的模板(DOM-based)、活动模板(Living Template)

##2.4.1 基于字符串的模板(String-based)

1、基于字符串的模板(String-based)，解决方案包括(dustjs、hogan.js、dot.js)
 
 
原理如下：输入一段模板字符串，通过编译之后 ，生成一段Function，通过Function的render或类render函数渲染输入的数据data，输出模板字符串，字符串通过innerHTML或类似的方式渲染成最后的DOM结构。这类模板的问题在于通过字符串生成DOM之后就不再变化，如果在改变输入的数据data，需要重新render，重新生成一个全新的DOM结构，性能较差。但该模板可以在服务器端运行
 


