# OfflineMap说明文档

---

**1. 基本说明**

OfflineMap实现了离线展示百度、谷歌、高德、腾讯地图的功能。主要功能如下：

 - 地图瓦片图直接可存储至[MySQL][1]数据库 
 - [Node.js][2]服务调用MySQL中的瓦片图 
 - [Leaflet][3]展示地图

展示效果如下：

![展示效果][4]

**2. 地图瓦片下载工具及配置**

工具下载链接: http://pan.baidu.com/s/1qYoHj4K 密码: ehgh
工具使用方法：

 - 数据库配置
 打开目录中的 MapDownloader.exe.config 文件。根据实际情况填写如图中的配置信息。
 ![数据库配置][5]

 - 地图瓦片图下载
 打开MapDownloader.exe -> 选择画图工具、矩形 -> 地图上框选区域 -> 存储方式选择MySQL数据库 -> Zoom根据需要选择 -> 点击下载
![下载瓦片图][6]

 - 数据库中存储的瓦片图
 ![数据库中存储的瓦片图][7]
 
> 备注：此工具功能丰富，可自己再细细研究。

**3. node.js服务配置**

 - mysql插件安装。在此项目目录内运行 `npm install mysql`
 - 在目录内运行 `node index.js`
 - 以上运行完毕后，默认服务地址：http://127.0.0.1:3001

**4. 页面展示**

打开example文件夹中的map.html即可。

**如本项目对您有所帮助，欢迎Star。**


  [1]: https://www.mysql.com/
  [2]: https://nodejs.org/en/
  [3]: http://leafletjs.com/
  [4]: http://i2.kiimg.com/561545/216983d692fef56a.jpg
  [5]: http://i2.kiimg.com/561545/18b1c776ce529746.jpg
  [6]: http://i4.piimg.com/561545/30fdee742409cee8.jpg
  [7]: http://i4.piimg.com/561545/1f87b80cce9a7c26.jpg