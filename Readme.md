---
layout: post
title: 飞享项目说明
category: IM
description: 
---

# 项目概述
为了便于项目的管理与发展,将项目相关的仓库全部移动到这里.之前在[github](https://github.com/comsince),[gitee](https://gitee.com/)的个人账户下面的项目,原则上全部移动到这里维护

# 项目列表
* [chat-server-release](https://github.com/fsharechat/chat-server-release) 飞享服务端发布项目,便于快速本地部署
* [chat-server](https://github.com/fsharechat/chat-server)  IM服务端项目
* [android-chat](https://github.com/fsharechat/android-chat) Android客户端项目
* [vue-chat](https://github.com/fsharechat/vue-chat)  基于vue的web端项目
* [vue-mobile-chat](https://github.com/fsharechat/vue-mobile-chat) 基于vue的移动端项目
* [electron-chat](https://github.com/fsharechat/electron-chat) 基于electron的pc端项目
* [chat-proto](https://github.com/fsharechat/chat-proto) 基于protobuf的相关proto定义文件

**NOTE:** 有些项目由于商业原因,有可能你无法访问.添加权限请联系QQ `1282212195`


# 项目演示说明

* [vue-chat-web版本](https://chat.comsince.cn/)
* [vue-mobile-chat移动版本](https://chat.comsince.cn/mobile)
* Android扫码下载  
![image](https://media.comsince.cn/minio-bucket-image-name/1-373z3zNN-1594953226715-fshare-chat-apk-qrcode.png)

**NOTE:** 由于现在没有开通短信功能,可以使用下演示帐号登录

```shell
帐号：13800000000, 13800000001, 13800000002
验证码：556677
```

## 项目迁移问题
**NOTE:** 针对项目改变地址,可以使用以下方法快速切换代码拉取地址,以下以`chat-server-release`具体说明,其他项目基本类似
```shell
git remote rm origin
git remote add origin git@github.com:fsharechat/chat-server-release.git
## 同步以下主干分支提交
git branch --set-upstream-to=origin/master
```

# 文档列表
## 技术说明
* [飞享-即时聊天系统技术文档](https://www.comsince.cn/2020/05/18/universe-push-tech-doc/)
## 部署
* [即时聊天系统在Centos上单机部署实践](https://www.comsince.cn/2020/04/13/universe-push-start-on-centos/)
* [即时聊天系统在Windows上单机测试部署实践](https://www.comsince.cn/2020/05/07/universe-push-start-on-windows/)
## 音视频方案
* [实时音视频开发的工程化实践](https://www.comsince.cn/2020/03/04/web-rtc/)
* [多人音视频会话方案预研](https://www.comsince.cn/2020/06/01/muti-conference-webrtc/)


# 功能列表

<table>
    <tr>
        <th>主功能</th>
        <th>功能说明</th>
        <th>web</th>
        <th>h5</th>
        <th>android</th>
    </tr >
    <tr>
        <td >登录</td>
        <td>支持腾讯云,阿里云验证码登录</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td rowspan="2">用户信息</td>
        <td>修改用户头像</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td>修改用户昵称</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td rowspan="4">好友列表</td>
        <td>发送好友请求</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td>处理好友请求</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td>修改好友备注名</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td>好友列表查看</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td rowspan="5">单聊</td>
        <td>文本/视频/图片</td>
        <td>√</td>
        <td>√</td>
        <td>√</td>
    </tr>
    <tr>
        <td>语音</td>
        <td>×</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>消息删除</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>消息撤回</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>消息转发</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td rowspan="7">群聊(含基本单聊功能)</td>
        <td>群聊创建</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>修改群名称</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>群聊退出</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>群聊解散</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>群成员列表</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>成员邀请</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>成员删除</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td rowspan="2">实时音视频</td>
        <td>一对一音视频</td>
        <td>√</td>
        <td>×</td>
        <td>√</td>
    </tr>
    <tr>
        <td>群组音视频</td>
        <td>√</td>
        <td>×</td>
        <td>×</td>
    </tr>
    
</table>

# 商业说明

## 一次性赞助

但是随着项目的增长，也需要相应的资金支持，你可以通过以下方式来赞助此项目

| 支付宝      | 微信| 
| :--------: | :--------:| 
|<img src="https://media.comsince.cn/minio-bucket-image-name/zfb-purse.jpg" alt="图片替换文本" width="300" height="450" align="center" />|<img src="https://media.comsince.cn/minio-bucket-image-name/wx-purse.png" alt="图片替换文本" width="300" height="450" align="center" />|

## 技术支持

如果公司采用本项目或者需要有商业需求，需要二次开发,提供技术支持,联系QQ：`1282212195`