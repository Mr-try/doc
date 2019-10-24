---
title: charles使用注意事项
date: 2019-10-16 17:54:13
tags:
---
# 

- 关闭代理，以免端口冲突
- pc端代理https的时候需要安装charles https证书
- 移动端网页调试的时候 如果是网页则pc端安装https证书即可
- 如果是app抓包
  - 一种方式是android>6的时候需要在构建app的时候开放对应的权限
  - 另一种是root后把Charles的http证书安装到系统证书中去，如果root则只能安装到用户证书不能抓取https
- facebook有一款app调试的工具[flipper](https://github.com/facebook/flipper),可以针对正在开放的application
   进行layout、crash、network等进行分析，前提需要在构建app的时候需要将对应的工具包打包进去