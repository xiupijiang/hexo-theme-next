title: MySQL流行的原因
date: 2016-09-07 04:14:22
author: xiupi酱
categories: 后端
tags: [MySQL, mysql]
---
## 简单


尽管MySQL源码的入门门槛很高，很多人不能深入其中，但是MySQL的使用还是非常简单的，任何稍微有IT背景的技术人员都可以无师自通地参照文档安装运行和使用MySQL,这几乎没有什么门槛。同时，MySQL支持大部分ANSI SQL-92，略有经验的使用者都能完成基本的操作需求。

## 开源

开源意味着安全和免费，代码就摆在那里，无数的技术爱好者一起来审核程序，一起修补问题，这让使用者非常的放心。同时，开源带来了免费。从上世纪90年代末一直持续到现在，互联网的兴起并快速发展，对免费数据库的需求非常迫切，免费，也让规模化部署的需求成为可能。要知道很多大型互联网公司的MySQL集群都是数以千记或者万记的，如果是按照传统的商业数据库的收费模式，没有人愿意承担。免费，让数据库大规模使用成为可能，也提升了互联网的交互式服务的质量。

## 复制

MySQL从3.23.15这个版本开始，支持了replication，可以帮助MySQL使用者搭建Master-Slave的架构。把数据准实时的从一个实例同步到另一个实例。这个时间是2000年之前。要知道，其他一些开源数据库是在最近的几年里才开始支持这样的功能的,这对于数据库使用者来说，不管是在线备份还是读写分离，或者负载均衡到多个读库，意义实在太大了。

在2010年之前，一个Master，多个slave的部署情况随处可见，我见过有12个slave的情形，可以设想，如果没有replication功能，我们要用数据库处理百万甚至是亿万规模的查询负载是非常困难的。

## 引擎

MySQL不同于其他多数数据库之处是它对插件式存储引擎的支持，这是一个开放的设计，有点兼容并包，海纳百川的感觉。熟悉MySQL的人随便就能报出几种MySQL存储引擎的名字，MyISAM，InnoDB，NDB,TokuDB，等等。

而MySQL里最常用的，也是奠定了MySQL开源数据库之王地位的InnoDB，并不是Monty或者他的伙伴们开发的。插件式存储引擎的设计，让InnoDB以及其他存储引擎轻松接入到MySQL Server，集百家之长，这样MySQL就有了无限的活力和竞争力以保持其长盛不衰。

## 支持

Monty说在早期MySQL刚刚推出的时候，他亲自写了30000封邮件来帮助人们使用MySQL。这样持之以恒，不辞劳苦，不厌其烦的精神让人赞叹。我们自己也维护了一个开源数据库项目InceptionSQL审核。在过去的一年多里，我们也碰到了很多很多的使用者提问的问题，这种感受，真的是只有经历过才能体会其中的付出。

## 合作

MySQL在发布的早期，就广泛的跟其他社区合作，PHP和Perl的开发者都很愿意去传播MySQL的技术和新闻，很多Linux版本都会预装MySQL。一度LAMP（Linux，Apace，MySQL，Php）成为站长或者开发者的标配。MySQL在各种合作中逐步深入人心,遍地开花。
**关注一下；你就知道**
![关注一下；你就知道][1]


  [1]: http://od3jhy35s.bkt.clouddn.com/ewm.jpg