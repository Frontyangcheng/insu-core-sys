#工具包
工具包(Utililty)的主要职责包括以下：

1、提供 JavaScript 原生不提供的功能

2、包装原生方法，使其便于使用

3、异步队列及流程控制



**常用的工具包解决方案**

有es5-shim、es6-shim、underscore、Lodash等；

上面提到的shim，也是经常听到的一个词，翻译过来是垫片的意思。对于es5、es6等
标准包括的一些新方法，由于浏览器兼容性不高，所以无法直接使用它们。这时，就需要在保证实现与规范一致的基础上，来扩展原型方法，这种做法就叫做shim。好处在于，实际上就是在使用javascript的语法，但不用去考虑低版本浏览器的兼容性问题
es5-shim 提供 ES3 环境下的 ES5 支持
es6-shim 提供 ES5 环境下的 ES6支持
underscore 提供兼容 IE6+ 的扩展功能函数
Lodash是underscore 的高性能版本，方法多为 runtime 编译出来的
