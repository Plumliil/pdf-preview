# PDF PREVIEW

基于pdfjs 2.0.943 打包后文件结合 VUE3 而编写的一个简单的pdf预览器的示例组件.

使用时可以将public下的pdfjs文件夹复制到所需集成项目的public文件夹下

通过iframe更改src路径为`./pdfjs/web/viewer.html?file=xxx`即可预览


### 页面展示
全局搜索 `mark-li` 即可查看标记注释,方便快速定位页面下载,打印等按钮在html中的位置 来进行显示隐藏操作

### 事件拦截
全局搜索 `mark-li` 即可查看标记注释,方便快速定位页面下载,打印等按钮在html中的位置 来进行对应事件的注释拦截

### 电子签名

已将从CDN加载字体修改为加载本地文件夹字体,若签名仍不显示,可以考虑本地文件夹是否不存在该签名字体

全局搜索 `mark-li : 使用CDN加载签名字体` 即可修改配置

本地字体文件夹目录为 `public/pdfjs/web/cmaps`


### 预览地址

具体效果可查看 [Pdf Preview Demo](https://pdf.plumliil.cn/)