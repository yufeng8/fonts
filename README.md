# fonts
字体文件存档及引用


使用jsDelivr加速GitHub静态资源

CDN的全称是Content Delivery Network，即内容分发网络。CDN是构建在网络之上的内容分发网络，依靠部署在各地的边缘服务器，通过中心平台的负载均衡、内容分发、调度等功能模块，使用户就近获取所需内容，降低网络拥塞，提高用户访问响应速度和命中率。CDN的关键技术主要有内容存储和分发技术。——百度百科

为什么要使用他
GitHub静态资源访问很慢，利用jsDelivr来加速它！

由于各种因素，GitHub的速度总是差强人意。使用国内对象储存需要收费和备案，对非盈利性站点简直是雪上加霜。所以推荐jsDelivr，它是一款免费的CDN！

目前GitHub仓库容量是没有上限的！不过官方推荐在1G以内！仓库单个文件大于50M会收到警告，大于100M会被拒绝！jsDelivr仅能针对50M以下的文件CDN加速

放在Github的资源在国内加载速度比较慢，因此需要使用CDN加速来优化网站打开速度，jsDelivr + Github便是免费且好用的CDN，非常适合博客网站使用。

怎么用
在github中创建仓库，这个仓库单独用来存放你要使用的cdn资源。大佬也可以项目仓库单独分文件夹直接用
将本地文件上传到仓库，
找到code branch tag，点击tag，再点击release
进行release,版本号要写成1.0.0这样的
访问
公式 https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径)
@发布的版本号为可选内容，是为了区分新旧内容，默认引用最新资源
除此之外还可以使用某个范围内的版本，查看所有资源等，具体使用方法如下：
加载任何Github发布、提交或分支
https://cdn.jsdelivr.net/gh/user/repo@version/file

// 加载 jQuery v3.2.1
https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/dist/jquery.min.js

// 使用版本范围而不是特定版本
https://cdn.jsdelivr.net/gh/jquery/jquery@3.2/dist/jquery.min.js
https://cdn.jsdelivr.net/gh/jquery/jquery@3/dist/jquery.min.js

// 完全省略该版本以获取最新版本
https://cdn.jsdelivr.net/gh/jquery/jquery/dist/jquery.min.js

// 将“.min”添加到任何JS/CSS文件中以获取缩小版本，如果不存在，将为会自动生成
https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/src/core.min.js

// 在末尾添加 / 以获取资源目录列表
https://cdn.jsdelivr.net/gh/jquery/jquery/

最后
使用版本号：不管你是删除文件还是修改文件，内容就是那个发布版本的内容。
不使用版本号：没有版本的限制，需要频繁更新推荐使用。
————————————————
版权声明：本文为CSDN博主「JunYu_coding」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/qq_45505100/article/details/113060212
