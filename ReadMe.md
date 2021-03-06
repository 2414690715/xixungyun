### 说明

本项目为了解放双手而诞生，代码较为粗糙，大佬勿喷，喜欢请给个star，谢谢！

### 主要功能

#### 日报

默认每天20:00运行，可自定义上传内容，请参考config下的<a href="https://github.com/2414690715/xixungyun/blob/main/src/main/resources/config/day.properties">day.properties</a>

#### 周报

默认每过七天运行一次，可自定义上传内容，请参考config下的<a href="https://github.com/2414690715/xixungyun/blob/main/src/main/resources/config/week.properties">week.properties</a>

#### 月报

默认每月20号18点运行，可自定义上传内容，请参考config下的<a href="https://github.com/2414690715/xixungyun/blob/main/src/main/resources/config/month.properties">month.properties</a>

#### 每日签到

默认每天6点运行，支持<a href="https://github.com/2414690715/xixungyun/blob/main/src/main/resources/config/everydaysign.properties">自定义</a>地点和经纬度，经纬度获取请前往<a href="https://lbs.amap.com/tools/picker">here</a>

#### 健康日报

默认每天8点运行，健康参数都为健康（除非你不健康）否则不是很需要定义参数，只需填写紧急联系人和手机号。

#### 推送

完成了什么功能会推送到手机上，详情请往下看。

### 命令行运行

```bash
java -jar xixunyun-0.0.1-SNAPSHOT.jar --xixunyun.username=习讯云账号 --xixunyun.password=密码 --pushplus.token=推送token --xixunyun.familyName=紧急联系人姓名 --xixunyun.familyPhone=紧急联系人电话
```

### pushplus

pushplus(推送加)是集成了微信、企业微信、钉钉、短信、邮件等渠道的信息推送平台

只需要调用一个简单的API接口，即可帮助你迅速完成消息推送，使用简单方便

我们的所做的一切只是为了让推送变的更简单（复制自<a href= "https://pushplus.plus/">官网</a>）

![image-20220512212156872](https://cdn.jsdelivr.net/gh/2414690715/imgPool/img/2022051261814805c3c2fe472fff1d7d0316ba51-1719b3.png)

微信扫码登录复制你的token

### Docker

![image-20220513121210017](https://cdn.jsdelivr.net/gh/2414690715/imgPool/img/202205130e1bf578e25a836b45f466fcf25dcaea-a5cd17.png)

修改Dockerfile文件：

```bash
把Dockerfile和Jar包单独放到一个文件夹
# cd /opt
# mkdir xixunyun
# cd xixunyun
# docker build -t 镜像名字 .
```

### 参数详解

详情请参考配置项目文件
