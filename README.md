
[面试](https://github.com/stevenli91748/Distributed-System/tree/master/Interview)
---

目录
-----

<a href="https://ibb.co/Yd8D2mY"><img src="https://i.ibb.co/Ks7N6dR/image.jpg" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>upload image</a><br />

<a href="https://imgbb.com/"><img src="https://i.ibb.co/qFQZzy9/image.jpg" alt="image" border="0"></a>


<a href="https://ibb.co/7YrpfWW"><img src="https://i.ibb.co/xCzgkjj/image.png" alt="image" border="0"></a>

[架构师的成长之路，第一步该怎么迈？我给大家准备好了](https://zhuanlan.zhihu.com/p/336838942)|
---|


[两万字深度介绍分布式系统原理，一文入魂](https://www.cnblogs.com/luckcs/articles/11235559.html)|[「分布式系统理论」系列专题，历时9个月完结](https://mp.weixin.qq.com/s?__biz=MzA3ODIxNjYxNQ==&mid=2247487132&amp;idx=1&amp;sn=24b36143d7ab742ad1ff4b23d8dec0a3&source=41#wechat_redirect)|[一步一图，带你了解分布式架构的前世今生](https://developer.51cto.com/art/201906/597667.htm)|
---|---|---|

[分布式系统各个节点状态如何同步](https://zhuanlan.zhihu.com/p/159136843?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)|[Vagrant---分布式开发的环境配置工具](https://jimmysong.io/blog/vagrant-intro/)|
---|---|

[疯狂创客圈 IM---从0开始100w分布式 Java 高并发、分布式应用实战](https://gitee.com/crazymaker/crazy_tourist_circle__im)|
---|

[分布式高性能高可用架构到底怎么做](https://zhuanlan.zhihu.com/p/145015244)|[分布式系统CAP选择](https://www.yuque.com/yulongsun/java/ugg3tt)|
---|---|

# [分布式系统的技术栈](https://zhuanlan.zhihu.com/p/336838942)

**且不说远程方法不能再依靠本地方法那些以内联为代表的传统编译优化来提升速度，光是“远程”二字带来的网络环境下的新问题，譬如，远程的服务在哪里（服务发现），有多少个（负载均衡），网络出现分区、超时或者服务出错了怎么办（熔断、隔离、降级），方法的参数与返回结果如何表示（序列化协议），信息如何传输（传输协议），服务权限如何管理（认证、授权），如何保证通信安全（网络安全层），如何令调用不同机器的服务返回相同的结果（分布式数据一致性）等一系列问题**

  * 分布式通信技术---因为业务拆分的多，业务对应的模块之间就需要通信，为了保证通信的快速可靠，我们需要掌握分布式通信技术
    * RPC
    * MQ
    * 共享存储
  * 分布式资源管理和负载调度技术---业务拆分的过多，每个模块可能还需要搞集群，那么多服务器资源，为了能够保证资源的精准分配，我们还需要考虑分布式资源管理和负载调度技术
    * YARN
    * MESOS
    * TORCA
  * 分布式协调与同步技术---业务拆分之后，模块与模块之间又需要对很多共享数据做访问，为了保证安全完整的数据状态，我们也要用到分布式协调与同步技术
    * ZOOKEEPER
    * CONSUL
    * ETCD
  * 分布式存储技术---到了业务拆分的阶段，数据必然庞大，为了数据存储的可靠，为了保证优秀的数据读写性能，我们需要分布式存储技术
    * HDFS
    * CEPH
    * SWIFT
  * 分布式计算技术---业务如此复杂，为了公司的发展，业务能继续扩大，就需要能更加精准的营销和运营，我们还需要对数据进行实时、离线处理分析，此时，我们又得考虑分布式计算技术
    * MAPREDUCE
    * STORM
    * FLINK
  * 分布式的可靠性技术---在业务拆分后，整体架构出现了巨变，不可能再用以前集群方式的思维去考虑高可用，那么分布式的可靠性技术又要纳入我们的掌握范畴
    * 负载均衡
    * 流量控制
    * 故障隔离
  
# [0. 分布式中间件技术](https://github.com/stevenli91748/Distributed-System/blob/master/%E5%88%86%E5%B8%83%E5%BC%8F%E4%B8%AD%E9%97%B4%E4%BB%B6/README.md)
# [1. 分布式系统基础知识](https://github.com/stevenli91748/Distributed-System/tree/master/Fundametal%20knowledge)

# [2. 分布式系统架构体系](https://github.com/stevenli91748/Distributed-System/tree/master/Architecture)

 *  基于对象的体系结构
 *  面向服务的架构 （SOA）
 *  REST 风格的架构
 *  微服务架构 (MSA)
 *  容器技术架构
 *  Serverless 架构


#  [3. 分布式系统的种类](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/README.md)

## [1. 分布式操作系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distributed%20operation%20system/README.md)

## [2. 分布式缓存系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/distribute%20cache/README.md)
 *  分布式缓存的实现
 *  [Redis](https://github.com/stevenli91748/Database/blob/master/Redis/README.md)

## [3. 分布式计算系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/distribute%20computing%20system/README.md)
 *  MapReduce
 *  Hadoop
 *  Spark
 *  Mesos
 
## [4. 分布式文件系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distribute%20file%20system/README.md)
 *  分布式文件系统的实现

## [5. 分布式存储系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distribute%20storage%20system/README.md)
 *   Bigtable
 *   HBase
 *   Cassandra
 *   Memcached
 *   MongoDB
 
## [6. 分布式消息服务系统](https://github.com/stevenli91748/Message-Server-System/blob/master/README.md)
 *   分布式消息队列的实现
 *   ActiveMQ
 *   RabbitMQ
 *   RocketMQ
 *   kafka

## [7. 分布式监控](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distribute%20moniter%20system/README.md)
 *   Nagios
 *   Zabbix
 *   Consul
 *   [分布式链路追踪](http://bigbully.github.io/Dapper-translation/)
     * [蚂蚁金服分布式链路跟踪组件 SOFATracer 总览](https://www.sofastack.tech/blog/sofa-tracer-overview/)
     * Pinpoint
     * [twitter zipkin](https://zipkin.io/)
     * [阿里的鹰眼](https://www.slideshare.net/terryice/eagleeye-with-taobaojavaone)
     * [美团的MTrace](https://tech.meituan.com/2016/10/14/mt-mtrace.html)
 *   [Apache SkyWalking](http://skywalking.apache.org)---Application performance monitor tool for distributed systems, especially
                                                         designed for microservices, cloud native and container-based (Docker, K8s,
                                                         Mesos) architectures.
     * [全面的深入学习Skywalking](https://www.bilibili.com/video/BV1ZJ411s7Mn?from=search&seid=4920628030984643892)
     
## [8. 分布式协调 ](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distributed%20coordination/README.md)
 *   [Zookeeper](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distributed%20coordination/Zookeeper.md)
 
## [9. 分布式版本控制系统](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/Distribute%20version%20control/README.md)
 *   Bazaar
 *   Mercurial
 *   Git
 
## [10. 分布式事务](https://github.com/stevenli91748/Distributed-System/blob/master/type%20of%20system/transection/分布式事务.md)

## [11. 分布式锁]()

## [12  分布式搜索系统]()

## [13. 分布式配置中心]()

## [14. 分布式日志中心]()

## [15. 分布式监控告警中心]()

## [16. 分布式会话]()

   * [阿里P8架构师谈：分布式Session共享的4类技术方案，与优劣势比较](https://youzhixueyuan.com/4-kinds-of-schemes-for-distributed-session-sharing.html)
   
## 17 分布式ID   
## 18 分布式任务调度
## 19 分布式限流
## 20 分库分表

#  [4. 分布式服务框架](https://github.com/stevenli91748/Distributed-System/tree/master/Service%20framework)

## [4.1  常用的 RPC 框架](https://github.com/stevenli91748/Distributed-System/blob/master/Service%20framework/RPC.md)

##  4.2  Dubbo

##  4.3  Spring Cloud




# 分布式视频
 * [项目搭建“天眼”Java大规模分布式跟踪监控系统（实战项目）](https://www.bilibili.com/video/BV1gZ4y1x7VM?p=6)
 * [大型分布式网站架构技术](https://www.bilibili.com/video/av64277303)
 * [阿里P8推荐】B站最全最详细的分布式架构学习视频全集](https://www.bilibili.com/video/BV1aJ411Y73e/?spm_id_from=333.788.videocard.2)
 * [B站最全最详细的分布式架构学习视频全集](https://www.bilibili.com/video/BV1aJ411Y73e/?spm_id_from=333.788.videocard.0)
 * [分布式基础专题](https://www.bilibili.com/video/av65840085/?spm_id_from=333.788.videocard.19)
 * [Java分布式进阶](https://www.bilibili.com/video/av58251897/?spm_id_from=333.788.videocard.10)
 * [中华石杉老师-21天互联网Java进阶面试训练营（分布式篇](https://www.bilibili.com/video/av71506934/?spm_id_from=333.788.videocard.15)
 * [分布式技术难点解决方案](https://www.bilibili.com/video/av63568054/?p=19)
 * [Java分布式锁没那么简单,并发量暴增我们的锁怎么办](https://www.bilibili.com/video/av69188361)
 * [从零开始 全面揭秘分布式任务调度](https://www.bilibili.com/video/av37409563/?spm_id_from=333.788.videocard.10)
 * [最牛Java分布式架构全套视频教程](https://www.bilibili.com/video/av63095169?p=6)
 * [阿里神秘技术内幕解密~分布式架构下的数据一致性技术解析](https://www.bilibili.com/video/av38331384?from=search&seid=5320849185764424951)
 * [微服务架构需要解决的各种问题--Dubbo Zookeeper Nginx API网关 ](https://www.bilibili.com/video/av65833021?p=13)
 * [千锋Java：分布式基础知识点教程](https://www.bilibili.com/video/av45732297?from=search&seid=15013736168332447863)
 * [java高并发分布式SSM项目实战](https://space.bilibili.com/7028047/channel/detail?cid=40223)
 * [[全面]JAVA分布式架构师项目实战Springboot+MyBatis+RocketMQ+Zookeeper](https://www.bilibili.com/video/av46875560/?spm_id_from=333.788.videocard.10)
 * [大型分布式项目项目实战系统架构+数据库设计+各类支付方式详解+实战大型](https://www.bilibili.com/video/av70430062?from=search&seid=1230906880023099423)
# 参考书籍

 * 人人都是架构师  分布式系统架构落地与瓶颈突破
 * 架构解密.从分布式到微服务
 * 亿级流量网站架构核心技术+跟开涛学搭建高可用高并发系统
 * 分布式操作系统----第一部
 * 分布式系统原理与范型---第二部
 * 深入分布式缓存 从原理到实践
 * 分布式系统常用技术及案例分析
 * 大规模分布式系统架构与设计实战
 * 大型分布式网站架构设计与实践
 * 大型网站系统与Java中间件实践
 * 分布式Java应用：基础与实践
 * 大型网站技术核心原理与案例分析
 
 # 有用的参考
 * [看一眼就能懂的“分布式锁”原理](https://developer.51cto.com/art/201906/597620.htm)
 * [我个人的分布式集群问题集锦，nginx/lvs/dns/cdn](https://blog.csdn.net/libaineu2004/article/details/79119145)
 * [强！强！强！13张图彻底搞懂分布式系统服务注册与发现原理](https://www.jianshu.com/p/e882e535a6b3)
 * [面试官问了我分布式事务](https://www.jianshu.com/p/70e4ca5e7c53)
 * [数据库并发控制](https://zhuanlan.zhihu.com/p/168672853?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656&utm_content=first)
 * [分布式缓存架构设计](https://www.jianshu.com/p/39c9a48bd704)
 * [一口气说出9种分布式ID生成方式，阿里面试官都懵了](https://zhuanlan.zhihu.com/p/152179727?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656&utm_content=first)
 * [这几种常见的“分布式锁”写法，搞懂再也不怕面试官](https://www.jianshu.com/p/07614d9542c4)
 * [ Mesos， Docker， Marathon/Chronos,  RabbitMQ,  HDFS/Ceph构成了一个完整的分布式系统](https://blog.csdn.net/hackstoic/article/details/50574886)
 * [2020 Java面试题最新(七分布式篇)](https://blog.csdn.net/weixin_43291173/article/details/104282183)
 * [为什么要用分布式架构，又为什么要用微服务](https://blog.csdn.net/world6/article/details/79114105)
 * [一分钟弄懂什么是分布式和微服务](https://blog.csdn.net/zhonglunsheng/article/details/83153451)
 * [一篇读懂分布式架构下的负载均衡技术：分类、原理、算法、常见方案等](http://www.52im.net/thread-2494-1-1.html)
 * [新手入门：零基础理解大型分布式架构的演进历史、技术原理、最佳实践](http://www.52im.net/thread-2007-1-1.html)
 * [腾讯资深架构师干货总结：一文读懂大型分布式系统设计的方方面面](http://www.52im.net/thread-1811-1-1.html)
 * [IT技术精华网关注搜索、分布式系统、云计算、系统架构设计、性能调优、Web开发、数据挖掘、推荐系统](http://www.chepoo.com)
 * [（重点）深入理解Java分布式架构](https://blog.csdn.net/yifanSJ/article/details/79098855)
 * [Java程序员进阶必知的分布式系统专业术语分析](https://blog.csdn.net/javaxuexi123/article/details/80508935)
 * [分布式系统(Distributed System)资料](https://www.bbsmax.com/A/obzbk3LMJE/)
 * [架构设计分布式技术干货整理](https://mp.weixin.qq.com/s/Wd73-YkbiKFVtuc0Ripn0Q)
 * [Zookeeper 集群安装配置，超详细，速度收藏](https://mp.weixin.qq.com/s/5APHlfBgNIwrIUPaPjw6qQ)
 * [我们来谈下高并发和分布式中的幂等处理](https://juejin.im/post/5c05f233e51d4524860fc51a)
 * [java实现分布式项目搭建的方法](https://www.jb51.net/article/138615.htm)
 * [Java系统的高并发解决方法详解](https://www.jb51.net/article/124145.htm)
 * [java 分布式与集群的区别和联系](https://www.jb51.net/article/105828.htm)
 * [详解Java如何实现基于Redis的分布式锁](https://www.jb51.net/article/91484.htm)
 * [Java分布式锁的三种实现方案](https://www.jb51.net/article/103617.htm)
 * [java高并发写入用户信息到数据库的几种方法](https://www.jb51.net/article/107279.htm)
 * [Java使用代码模拟高并发操作的示例](https://www.jb51.net/article/139429.htm)
 * [WHAT WE TALK ABOUT WHEN WE TALK ABOUT DISTRIBUTED SYSTEMS](http://alvaro-videla.com/2015/12/learning-about-distributed-systems.html)
 * [亿级Web系统搭建：单机到分布式集群](https://blog.csdn.net/u013256816/article/details/48707505)
 * [还不理解“分布式事务”？这篇给你讲清楚！](https://cloud.tencent.com/info/7aee761848382a55d59b6619849abf64.html)
 * [分布式系统关注点——想通关「限流」？只要这一篇](https://cloud.tencent.com/info/03caa5eae776645a87cb6304d33c5ba2.html)
 * [分布式ID生成器的解决方案总结](https://mp.weixin.qq.com/s/cTocuZg6Vm3G1EaPtu544w)
 * [深入理解分布式事务,高并发下分布式事务的解决方案](https://blog.csdn.net/mine_song/article/details/64118963)
 * [常用的分布式事务解决方案介绍有多少种？](https://blog.csdn.net/yanpenglei/article/details/79125578)
 * [分布式系统的唯一id生成算法你了解吗](https://juejin.im/post/5c6be4086fb9a04a060570df)
 * [一个比较不错的大型分布式网站架构技术总结，可做参考](https://blog.csdn.net/hjm4702192/article/details/79612611)
 * [分布式之消息队列复习精讲](http://www.cnblogs.com/rjzheng/p/8994962.html?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
 * [我理解的分布式系统](https://blog.csdn.net/lpd_tech/article/details/88122062)
 * [分布式 实战（干货）](https://blog.csdn.net/qq_27384769/article/details/79439782)
 -石杉的架构笔记

* [拜托，面试请不要再问我TCC分布式事务的实现原理！--石杉的架构笔记](https://mp.weixin.qq.com/s/mIW1_K5fAoa2OlSLdXSHpQ)
* [【坑爹呀】最终一致性分布式事务如何保障实际生产中99.99%高可用？--石杉的架构笔记](https://mp.weixin.qq.com/s/yRDUQtVPz5eqCx961xL6nw)
* [拜托，面试请不要再问我Redis分布式锁的实现原理！](https://mp.weixin.qq.com/s/y_Uw3P2Ll7wvk_j5Fdlusw)
* [每秒上千订单场景下的分布式锁高并发优化实践！](https://mp.weixin.qq.com/s/RLeujAj5rwZGNYMD0uLbrg)
* [【七张图】彻底讲清楚ZooKeeper分布式锁的实现原理！](https://mp.weixin.qq.com/s/jn4LkPKlWJhfUwIKkp3KpQ)
* [【温故知新】分布式事务及分布式锁系列文章总结](https://mp.weixin.qq.com/s/DltfG12wVttIyDUayeaL_A)
* [兄弟，用大白话给你讲小白都能看懂的分布式系统容错架构](https://mp.weixin.qq.com/s/DKf63ZDJQKoEiOmGqn3NxQ)
* [高并发场景下，如何保证生产者投递到消息中间件的消息不丢失？](https://mp.weixin.qq.com/s/r2_o5wa6Gn94NY4ViRnjpA)
* [面试大杀器：消息中间件如何实现消费吞吐量的百倍优化？](https://mp.weixin.qq.com/s/vZ4KVC2eGmssnQUyIKgzfw)
* [分布式之消息队列复习精讲](http://www.cnblogs.com/rjzheng/p/8994962.html?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
* [Java同学找工作最懵圈的问题：到底啥是分布式系统开发经验？](https://mp.weixin.qq.com/s/Z7jdt3yfINWV6NVl7u9PuA)
* [几种分布式调用技术的比较 -- RPC VS REST](https://blog.csdn.net/iter_zc/article/details/39341983)
* [JAVA中都有哪几种分布式实现方式,各有什么优缺点](http://www.dewen.net.cn/q/2430/JAVA中都有哪几种分布式实现方式%2C各有什么优缺点)
* [SkyWalking jvm指标采集与存储](https://blog.csdn.net/dw147258dw/article/details/93711710)
* [超详细！CentOS 7 + Hadoop3.0.0 搭建伪分布式集群](https://www.cnblogs.com/thousfeet/p/8618696.html)


