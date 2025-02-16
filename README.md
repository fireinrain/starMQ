# StarMQ1.0

## 介绍

- 本系统是为个人用户设计的收款免签约解决方案
- 拒绝高风险的扫码登录方式，采用 APP 监听系统收款通知方案，更安全可靠！
- 基于[ThinkPHP](https://www.thinkphp.cn/)框架开发

## 运行环境

- `PHP 8.0` PHP 版本向下兼容至 7.4(经过测试)
- `MySQL 5.7` MySQL 版本向下兼容至 5.6(经过测试)
- `Nginx 1.20.2`

## 预览

![](https://cdn.wgbor.cn/uploads/2023/02/02/167532925963db7eebdb8c9.png)

## 安装教程

1. 下载程序
2. 上传程序至服务器
3. 导入 star.sql 至数据库
4. 修改程序`config/database.php`文件的数据库配置信息（如下图）
   ![](https://cdn.wgbor.cn/uploads/2023/02/02/167532567063db70e6d4724.png)
5. 访问域名即可！

## 视频教程

[视频地址](https://www.bilibili.com/video/BV1MY411D7vD/)

## Tips

- 默认账号密码为`admin` `123456`
- 项目运行目录选择 `public`
- 伪静态设置为`ThinkPHP`

```
location / {
	if (!-e $request_filename){
		rewrite  ^(.*)$  /index.php?s=$1  last;   break;
	}
}
```

- APP 监控软件为根目录的 StarMQ.apk
  [点击下载](./StarMQ.apk)

## 项目推荐

[CloudZA API 一款开源的 API 系统](https://github.com/iCloudZA/CloudZA_API)

## 捐赠

- 如果你觉得程序好用的话，不妨通过捐赠的方式支持我们持续更新~
<center style="display:flex;">
<img src="./wx.jpg" width="50%">
<img src="./ali.jpg" width="50%">
</center>

## 问题反馈

- 邮箱： `i@kain8.cn`
- QQ 群：`758107405`
- QQ：`1361582519`
