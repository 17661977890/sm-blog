<p align="center">
  <a href="https://blog.ameilin.com/" target="_blank" rel="noopener noreferrer">
  <img width="180" src="https://cdn.jsdelivr.net/gh/17661977890/picgo-file/sm10.jpg" alt="logo">
  </a>
</p>

<p align="center"> 
  <a href="https://github.com/17661977890/sm-blog/stargazers">
    <img src="https://img.shields.io/github/stars/17661977890/sm-blog?logo=ReverbNation&logoColor=rgba(255,255,255,.6)" alt="GitHub stars">
  </a>
  <a href="https://github.com/17661977890/sm-blog/actions?query=workflow%3ACI">
    <img src="https://github.com/17661977890/sm-blog/workflows/CI/badge.svg" alt="CI">
  </a>
  
  <a href="https://github.com/17661977890/sm-blog/actions?query=workflow%3AbaiduPush">
    <img src="https://github.com/17661977890/sm-blog/workflows/baiduPush/badge.svg" alt="baiduPush">
  </a>
</p>

<h2 align="center">sm-blog</h2>

## 介绍
1. 本站基于`vuepress`,在`vuepress-theme-vdoing`知识库博客主题的基础上进行修改。
2. 本站主要用于作为个人`知识管理工具` 和 `个性化博客`,以 Markdown 为中心的项目结构。
3. 本站部分静态图片资源使用了 `picgo`+ `github图床` + `jsDelivr CDN加速`，方便灵活快速。
4. 欢迎访问本站：https://blog.ameilin.com/ （或点击上方logo）

## 致谢
:heart:感谢`vuepress-theme-vdoing`[知识库兼博客站](https://xugaoyi.com/)


## 本地启动本项目
* 1、git clone https://github.com/17661977890/sm-blog.git
* 2、yarn install
* 3、yarn dev


## 部署本项目（基于github pages）

* 1、git clone https://github.com/17661977890/sm-blog.git
* 2、yarn install
* 3、npm run deploy # 执行部署脚本即可
* 4、无个人域名
   * 配置github pages即可，如图所示：
   ![image](https://cdn.jsdelivr.net/gh/17661977890/picgo-file/5ab2e407ddffe0eb52a69e1f01351cbd.png)
   * 项目中 config.ts 中的 base配置此时为 /sm-blog/
   * 此时访问 176619977890.githup.io/sm-blog/ 接口
5、有个人域名
  * 在云平台配置域名解析
  ![image](https://cdn.jsdelivr.net/gh/17661977890/picgo-file/198f7035b9dea1876e521e8a75a5686c.png)
  * 在github pages中配置 custome domain
  ![image](https://cdn.jsdelivr.net/gh/17661977890/picgo-file/20240530115121.png)
  * 注意: 此时需要注释掉项目中 config.ts 中的 base配置 -----> 为什么？ 下面会说明
  * 此时访问 https://blog.ameilin.com/ 即可


### github自定义域名部署注意事项
* 浏览器如何解释绝对路径以及基准路径的问题？
```
访问自定义域名（例如 blog.ameilin.com）
绝对路径解析：
当你访问自定义域名时，浏览器会将路径解析为相对于根域名的绝对路径。
例如，如果你在页面中引用了 /image.jpg，浏览器会将这个路径解析为 blog.ameilin.com/image.jpg，而不是 blog.ameilin.com/sm-blog/image.jpg。这是因为在绝对路径中，默认情况下是相对于根路径的。
直接访问 GitHub Pages 地址（例如 https://17661977890.github.io/sm-blog）
绝对路径解析：

当你直接访问 GitHub Pages 地址时，浏览器会将路径解析为相对于该地址的绝对路径。
例如，如果你在页面中引用了 /image.jpg，浏览器会将这个路径解析为 17661977890.github.io/image.jpg，而不是 17661977890.github.io/sm-blog/image.jpg。这是因为在绝对路径中，默认情况下是相对于当前路径的。
修改 basePath 的作用：

如果你在 GitHub Pages 网站中使用了基准路径（basePath），比如设置为 /sm-blog，那么在页面中的路径引用将会基于这个基准路径进行解析。
例如，如果你设置了基准路径为 /sm-blog，那么在页面中引用了 /image.jpg，浏览器会将这个路径解析为 17661977890.github.io/sm-blog/image.jpg。这样就能正确找到资源了。
结论
通过理解浏览器对路径的解析方式以及基准路径的作用，可以更好地理解在不同环境下页面中的路径引用和资源定位。在 GitHub Pages 中使用基准路径可以使页面在不同地址下正确加载资源，这对于网站的可移植性和可维护性是非常有帮助的。
```

## 如何通过本项目改造成自己blog网站
* 后续补充...

## :sparkling_heart:支持这个项目

如果你通过本站有所解惑并感觉良好，想要让博主继续知识库更新的话，你可以通过如下*任意* 方式支持我：

1. *Star* 并 分享这个项目 :rocket:
2. 通过以下二维码 一次性捐款。 我多半会买一杯 ~~咖啡~~ 茶。:tea:

谢谢！ :heart:

| 微信赞赏 | 微信 |
| :---: | :---: |
| <img src="https://cdn.jsdelivr.net/gh/17661977890/picgo-file/admire.jpg" alt="赞赏码" width=150> | <img src="https://cdn.jsdelivr.net/gh/17661977890/picgo-file/pay.jpg" alt="Wechat QRcode" width=150>|


## 许可证
[MIT](https://github.com/17661977890/sm-blog/blob/master/LICENSE)

Copyright © 2024 Bin Sun(17661977890)
