create-react-app 把webpack、babel等配置都封装到了依赖项目react-script中，所以你无法直观的看到这些配置。
你可以在项目下运行npm run eject，被隐藏的配置文件就会暴露到项目根路径下。
把请求转发到index.html原因是，你执行npm run start时，启动的webpack-dev-server，会加载react-script项目config文件夹下的配置（paths.js）,里面定义了请求的默认转发路径是public文件夹，自然就找到了public下的index.html。

[参考链接](https://www.cnblogs.com/axl234/p/8269018.html)
