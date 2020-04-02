## 说明
该项目为了节约学习源码的同学的时间，已经把构建好的 react 可调试源代码贡献上来，直接在浏览器运行就可以了。

## 步骤
浏览器打开 fixtures/packaging/babel-standalone/dev.html 直接可以调试，已在 setState 打好断点。

## 后续如何调试 React 源码
1. 先 yarn 一下
2. 全局安装打包工具 rollup
3. 本地构建：yarn build react/index,react-dom/index --type=UMD
4. 用浏览器打开打开demo：位置在 fixtures/packaging/babel-standalone/dev.html
5. 为了研究一下 React 调用 setState 前后发生了什么，在Component.prototype.setState这里已打一个断点，在浏览器查看函数运行和前后的调用栈。
