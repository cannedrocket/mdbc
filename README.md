# 介绍
欢迎使用电影数据库（MDBC）API. 请邮件 living.on.a.tropical.island@gmail.com ,或访问 https://github.com/cannedrocket/mdbc 申请
API密钥, 目前数据和系统处于早期阶段, 数据包含绝大多数已发行电影和剧集信息, 但中文化在进一步整理之中, 并非所有条目录都具有中文翻译. 
除图片及静态数据透过CDN加速外, 小部分服务host于太阳能供电的树莓派上, 台风季会有小部分服务降级.  
测试api_key为: ae86d25032527a25fe60cdec7a77ae5e , 这个key全局共享quota为10次/分钟, 所以不能保证随时可用. 
    
# api接口协议
目前兼容tmdb(The movie database) v3版本的常用接口, 所以使用kodi/emby或其他的刮削工具只需替换api服务地址和api_key即可.
    
# 认证
获取API密钥后，实例请求如下(将文本替换成您自己的API密钥)：`<<api_key>>`
``` curl
https://api.moviedatabase.cloud/3/movie/68646?api_key=<<api_key>>
```
