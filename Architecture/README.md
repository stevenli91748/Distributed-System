* 原始分布式时代
* 单体系统时代---基于对象的体系结构
* SOA 时代---面向服务的架构 （SOA）
* 微服务时代--- 微服务架构 (MSA)
* 后微服务时代--- 容器技术架构
* 无服务时代---Serverless 架构
* 分布式微服务架构中需要解决的问题 
  * 服务的注册发现
  * 跟踪治理
    * [注册中心的设计与实现](https://github.com/aCoder2013/blog/issues/32) 
    * [微服务分布式配置中心组件](https://github.com/stevenli91748/MicroService/blob/master/%E5%BE%AE%E6%9C%8D%E5%8A%A1%E5%88%86%E5%B8%83%E5%BC%8F%E9%85%8D%E7%BD%AE%E4%B8%AD%E5%BF%83%E7%BB%84%E4%BB%B6/README.md) 
      * 服务调用
      * 服务容错 
      * [服务网关](https://github.com/stevenli91748/MicroService/tree/master/%E5%BE%AE%E6%9C%8D%E5%8A%A1%E7%BD%91%E5%85%B3)
      * 链路追踪
    * 负载均衡
    * 故障隔离
    * 服务间远程调用
    * 传输通信
    * 伸缩扩展
    * 微服务应用安全——Security
      * 微服务认证授权 
    * 微服务之分布式事务解决方案
      * [Seata 分布式事务](https://github.com/stevenli91748/JAVA-Architecture/blob/master/JAVA%20Framework/Spring%20Cloud/Spring%20Cloud%20Alibaba%E5%A5%97%E4%BB%B6/Seata.md)
      * [亿级流量架构之分布式事务思路及方法](https://www.cnblogs.com/Courage129/p/14433462.html)
      * [亿级流量架构之分布式事务解决方案对比](https://www.cnblogs.com/Courage129/p/14443653.html) 
      * [微服务分布式事务之LCN、TCC特点、事务补偿机制缘由以及设计重点](https://www.cnblogs.com/Courage129/p/14528981.html)
      * [微服务下如何保证事务的一致性](https://weread.qq.com/web/reader/d9e327a07188b377d9eb7dake3632bd0222e369853df322)
        * Apache RocketMQ--RocketMQ事务消息中间件主要解决了生产者端的消息发送与本地事务执行的原子性问题


