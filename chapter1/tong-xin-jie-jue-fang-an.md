#常用通信方式


关于通信，主要包括XMLHttpRequest、Form、JSONP、Socket等
通信相关的解决方案主要用于提供以下操作

1、处理与服务器的请求与相应

2、预处理请求数据与响应数据 Error/Success 的判断封装

3、多类型请求，统一接口（XMLHttpRequest1/2、JSONP、iFrame）

4、处理浏览器兼容性


### 2.2.1  常用方案

除了jQuery等，其他常用的通信解决方案有Reqwest、qwest等
Reqwest支持JSONP，稳定性高，IE6+支持，CORS 跨域；
Promise/A 支持 异步，跨域，有非常好用的aioxs库等；
qwest代码少、支持XMLHttpRequest2、CORS 跨域、支持高级数据类型（ArrayBuffer、Blob、FormData）
 ```


### 2.2.2 专业领域

对于实时性要求较高的需求可以使用websocket , socket.io，它实时性高，支持二进制数据流，智能自动回退支持，且支持多种后端语言







