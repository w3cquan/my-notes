# webpack使用

### 如何使用webpack?

webpack分为全局和局部，开发中一般会给项目单独安装一个局部webpack。

在全局安装webpack：`npm install webpack@3.6.0 -g`

在项目中安装webpack：`cd进入对应目录， npm install webpack@3.6.0 --save-dev`

检查webpack版本：`webpack --version`



### 使用webpack进行打包

1. 直接用模块化的方式开发
2. 使用webpack打包只需要一条命令: `webpack '需要打包的文件路径' '要打包到的目标路径'`
3. 在html文件中引入打包好的js文件



### 更加规范的打包方式：

1. 一般会在项目的根目录进行初始化`npm init`，得到文件package.json。这里面会显示入口文件，脚本命令，安装的插件版本等各种信息。
2. 还需要创建一个叫做webpack.config.js的配置文件，在这里面可以自定义设置需要处理的文件路径，打包到的路径，打包后的文件名等。
3. 在package.json文件里面的"scripts"对象里可以自己写命令的脚本，比如说我设置一个"dev"为"webpack"，那么我在终端输入`npm run dev`时，就会执行"webpack"这条命令。
4. 在package.json里面设置好需要打包文件的路径，打包完成的路径，就可以输入"webpack"命令进行打包了。输入`npm run dev`执行"webpack", 也是一样的。
5. 那么我在package.json文件里面设置entry为./src/index.js，在output里设置将要打包到dist文件夹，在filename里设置bundle.js。意思是我将要把./src/index.js打包到dist/bundle.js里面去。
6. 在index.html里引入./dist/bundle.js，运行代码，就能看到模块化的效果了。











