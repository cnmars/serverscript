# golang 项目结构布局

## go 目录

## /cmd 

项目的主干，次目录应该足够简单

## /interenal 

内部的，不需要分享到外部的，这个属于golang 内部的一个特性，我们也会在好多开源项目中看到

## /pkg 

可复用的一些代码库

## /vendor 

vendor 模式的包，现在推荐的玩法是go modules 功能
服务应用模式

## /api 

关于openapi/swaggeer 规范的json 模式文件
web 应用模式

## /web 

静态web资源，服务器模版以及单页面应用。。。
通用应用

## /config 

配置文件模版或者more 嗯配置

## /init 

system init 管理的脚本

## /scripts 

构建，安装，分析等的脚本

## /build 

打包以及持续集成的

## /deployments 

关于iaas paas，以及部署的，也可以水用/deploy 命名

## /test 

关于程序测试的

其他目录

## /docs 

设计以及用户文档

## /tools 

项目的支持工具，工具可以从/pkg 以及/inteernal 导入

## /examples 

公共实例

## /thrid_party 

外部辅助工具和，或者其他三方工具

## /githooks 

git hooks

## /assets 

与代码库共享的（图像，徽标）

## /website

关于项目的website 文档，可以使用github pages 。。。
不应该用的目录

## ~~~~/src~~ 

~~以前好多项目使用的是src 模式，已经不推荐使用了~~