#核心系统
**一、环境配置与启动**
环境配置：
```
node@6.9.5、npm@5.3.0、vue@^2.4.2、vue-router@^2.2.0、vuex@^2.2.1

```

**环境搭建**
安装node
1)、下载node-v6.9.5-x64.msi双击安装(可安装到除c盘外的其它盘) 
2)、cmd命令中输入node-v，出现版本号则安装成功 
3)、由于国内网络原因安装node之后，请自行安装cnpm 地址：http://npm.taobao.org/


**启动**
1.从gitlab上获取到和聚宝的git地址  http://git@gitlab.polyhome.net:react/insu-core-sys.git
git clone 地址。
2.将代码down下来后 
在项目根目录中执行npm i 或者 cnpm i 
3.在项目根目录中执行 npm run dev 来启动项目 
如果出现端口冲突的错误，你可以在 /config/index.js 文件中找到启动端口。

**二、项目结构说明**

![](/assets/微信截图_20181019182942.png)