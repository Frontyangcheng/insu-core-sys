#框架选择

##前端MVC框架

通常前端技术选型最核心的决策点就是所谓的前端MVC框架，网上充斥着这类框架的对比文章，但是孰优孰劣仍然是萝卜白菜，各有所爱，说一句正确的废话就是：框架的选择要因地制宜，根据应用场景和团队实际情况来定。

目前热度最高的三大前端框架是Angular（2.0+）、React和Vue.js。三者都采用了组件化的思想，同一component的html、js、css组织在一起，组件化思想对早期绝对的“关注点分离”则文件分离思想是一定程度的矫正，利于组件的单独开发和复用，减轻了html、js，特别是css的全局污染问题。
Angular是由Google推出的基于TypeScript的MVVM框架，视图和模型双向绑定，通过指令增强模板的表达能力，同时可以自定义组件化的指令，支持依赖注入、注解。由于策略上的问题，Angular2.0不兼容AngularJS 1.0，因此，近两年Angular的活跃度有所下降，然而其内置完备的特性和工具让拥护者们认为它是一个企业级的JS框架。
React由Facebook主推，最显著的特点是一切以JS为中心，HTML和CSS都由JS代码生成，为此，还产生了一种新的语法：JSX，这跟Angular把JS以扩展标签的形式放到HTML中是完全相反的做法。React实现了Virtual DOM，在DOM频繁变化的场景下，性能有不错的表现。另外，React本身主要关注于视图层，并不是一个大而全的框架，由于React认为MVC架构在大规模应用场景下会导致状态的混乱，因此创新地提出了单向数据流（Unidirectional data flow）的概念，出现了状态管理的模式或框架，如Flux/Redux。
Vue.js是三者之中最年轻、最轻量的一个框架，由华裔程序员尤雨溪发起，也是主要关注视图部分，既支持双向绑定也可以单向绑定。Vue.js的模板语法有点类似于Angular，提供了一些内置标签。Vue.js支持单文件组件，也就是将html、js、css写到一个后缀为.vue的文件中，也支持Virtual DOM，性能表现在三者中最好。Vue.js可以使用Redux做状态管理，但也提供了自己的Vuex。
值得一提的是，上面三个主流框架都有对应的移动端方案，比如Angular对应的Ionic，React的React Native以及Vue对应的Weex（阿里开发）。
数据和视图的不同交互方式催生出几个不同的概念：MVC、MVP、MVVM以及单向数据流。
下图是2017年不同国家对几大框架使用情况的调查反馈。
  调查反馈。



![](/assets/mvc.png)