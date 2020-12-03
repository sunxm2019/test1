https://github.com/Vincent131499/Chinese-OCR3

https://blog.csdn.net/hancoder/article/details/106922139

https://www.pythonf.cn/read/129365
http://www.jeepxie.net/article/313504.html

vue开发

用cmd执行下面的命令

```cmd
npm install -g webpack
npm install -g @vue/cli-init
```



追加Path

```
C:\Users\sunxm\AppData\Roaming\npm
C:\Users\sunxm\AppData\Roaming\npm\node_modules\@vue\cli-init\node_modules\.bin
```



创建Vue项目

先建文件夹vue-demo

```
vue init webpack vue项目名
```

![image-20200912202758647](vue开发.assets/image-20200912202758647.png)



```
cd vue-demo
npm run dev

http://localhost:8080
ctrl+C
```



config\index.js

port: 8081



element UI : https://element.eleme.cn/#/zh-CN/component/installation

```
npm i element-ui
```

引入 Element:

在 main.js 中写入以下内容：

```
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';

Vue.use(ElementUI);
```



Vue.js Devtoolsの導入方法について

https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd/related








