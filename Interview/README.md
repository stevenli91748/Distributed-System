# [分布式面试](https://thinkwon.blog.csdn.net/article/details/105870730)


<details>
<summary>CAP理论详解</summary>
[Spring cloud应该怎么入门之CAP理论详解](https://www.zhihu.com/question/283286745/answer/763040709)
</details>


<details>
<summary>最大并发连接数</summary>
最大并发连接数：防火墙或代理服务器对其业务信息流的处理能力，是防火墙能够同时处理的点对点连接的最大数目；
</details>

<details>
<summary>最大会话数</summary>
所有用户要通过防火墙上网，要打开很多个窗口或Web页面发生的状态就叫做会话，防火墙所能处理的最大限额就交最大会话数。
</details>

<details>
<summary>1. 单机 分布式和集群的区别</summary>

分布式：一个业务分拆多个子业务，部署在不同的服务器上

集群：同一个业务，部署在多个服务器上

**单机结构**
我想大家最最最熟悉的就是单机结构，一个系统业务量很小的时候所有的代码都放在一个项目中就好了，然后这个项目部署在一台服务器上就好了。整个项目所有的服务都由这台服务器提供。这就是单机结构。那么，单机结构有啥缺点呢？我想缺点是显而易见的，单机的处理能力毕竟是有限的，当你的业务增长到一定程度的时候，单机的硬件资源将无法满足你的业务需求。此时便出现了集群模式，往下接着看。

**集群结构**
集群模式在程序猿界有各种装逼解释，有的让你根本无法理解，其实就是一个很简单的玩意儿，且听我一一道来。单机处理到达瓶颈的时候，你就把单机复制几份，这样就构成了一个“集群”。集群中每台服务器就叫做这个集群的一个“节点”，所有节点构成了一个集群。每个节点都提供相同的服务，那么这样系统的处理能力就相当于提升了好几倍（有几个节点就相当于提升了这么多倍）。但问题是用户的请求究竟由哪个节点来处理呢？最好能够让此时此刻负载较小的节点来处理，这样使得每个节点的压力都比较平均。要实现这个功能，就需要在所有节点之前增加一个“调度者”的角色，用户的所有请求都先交给它，然后它根据当前所有节点的负载情况，决定将这个请求交给哪个节点处理。这个“调度者”有个牛逼了名字——负载均衡服务器。集群结构的好处就是系统扩展非常容易。如果随着你们系统业务的发展，当前的系统又支撑不住了，那么给这个集群再增加节点就行了。但是，当你的业务发展到一定程度的时候，你会发现一个问题——无论怎么增加节点，貌似整个集群性能的提升效果并不明显了。这时候，你就需要使用微服务结构了。
分布式结构先来对前面的知识点做个总结。从单机结构到集群结构，你的代码基本无需要作任何修改，你要做的仅仅是多部署几台服务器，每台服务器上运行相同的代码就行了。但是，当你要从集群结构演进到微服务结构的时候，之前的那套代码就需要发生较大的改动了。所以对于新系统我们建议，系统设计之初就采用微服务架构，这样后期运维的成本更低。但如果一套老系统需要升级成微服务结构的话，那就得对代码大动干戈了。所以，对于老系统而言，究竟是继续保持集群模式，还是升级成微服务架构，这需要你们的架构师深思熟虑、权衡投入产出比。OK，下面开始介绍所谓的分布式结构。

**分布式结构**
就是将一个完整的系统，按照业务功能，拆分成一个个独立的子系统，在分布式结构中，每个子系统就被称为“服务”。这些子系统能够独立运行在web容器中，它们之间通过RPC方式通信。举个例子，假设需要开发一个在线商城。按照微服务的思想，我们需要按照功能模块拆分成多个独立的服务，如：用户服务、产品服务、订单服务、后台管理服务、数据分析服务等等。这一个个服务都是一个个独立的项目，可以独立运行。如果服务之间有依赖关系，那么通过RPC方式调用。这样的好处有很多：系统之间的耦合度大大降低，可以独立开发、独立部署、独立测试，系统与系统之间的边界非常明确，排错也变得相当容易，开发效率大大提升。系统之间的耦合度降低，从而系统更易于扩展。我们可以针对性地扩展某些服务。假设这个商城要搞一次大促，下单量可能会大大提升，因此我们可以针对性地提升订单系统、产品系统的节点数量，而对于后台管理系统、数据分析系统而言，节点数量维持原有水平即可。服务的复用性更高。比如，当我们将用户系统作为单独的服务后，该公司所有的产品都可以使用该系统作为用户系统，无需重复开发。

</details>

<details>
<summary> 分布式系统的有状态、无状态</summary>

 * [分布式系统的基本术语之有状态、无状态](https://blog.csdn.net/m0_37854817/article/details/79467716)

</details>

<details>
<summary>分布式ID生成器</summary>

 * [分布式ID生成器](https://soulmachine.gitbooks.io/system-design/content/cn/distributed-id-generator.html)

</details>

<details>
<summary>短网址系统(TinyURL)</summary>

 * [短网址系统(TinyURL)](https://soulmachine.gitbooks.io/system-design/content/cn/tinyurl.html)

</details>

<details>
<summary>定时任务调度器</summary>

 * [定时任务调度器](https://soulmachine.gitbooks.io/system-design/content/cn/task-scheduler.html)

</details>

<details>
<summary>API限速</summary>

 * [API限速](https://soulmachine.gitbooks.io/system-design/content/cn/api-rate-limiting.html)

</details>

<details>
<summary>线程安全的HashMap</summary>

 * [线程安全的HashMap](https://soulmachine.gitbooks.io/system-design/content/cn/hashmap.html)

</details>

<details>
<summary>最近一个小时内访问频率最高的10个IP</summary>

 * [最近一个小时内访问频率最高的10个IP](https://soulmachine.gitbooks.io/system-design/content/cn/top-k-frequent-ip-in-one-hour.html)

</details>

<details>
<summary>Key-Value存储引擎</summary>

 * [Key-Value存储引擎](https://soulmachine.gitbooks.io/system-design/content/cn/key-value-store.html)

</details>





















---

<details>
<summary>PageRank算法</summary>

 * [PageRank算法]()

</details>

<details>
<summary> 什么是分布式系统？</summary>



</details>

<details>
<summary>分布式系统你会考虑哪些方面？</summary>



</details>

<details>
<summary>从分布式系统部署角度考虑，分哪几层？</summary>



</details>

<details>
<summary>分布式系统设计你会考虑哪些策略？</summary>



</details>

<details>
<summary>最常见的数据分布方式是什么？</summary>

</details>

<details>
<summary>一致性，高可用，网络分区容忍性为何只能三选二</summary>

</details>

<details>
<summary>为什么网络分区容忍性必须要被考虑</summary>

</details>

<details>
<summary>CAP在实际应用中真的可靠么？</summary>

</details>

<details>
<summary>BASE出现的原因</summary>

</details>

<details>
<summary>为什么BASE更容易实现，更适合实际应用</summary>

</details>

<details>
<summary>BASE可以通过哪些技术去实现呢？</summary>

</details>

高并发，高可用，海量数据，没有分布式的架构知识肯定是玩不转的所以分布式的知识需要掌握：

分布式架构思维

大型互联网架构演进过程

架构师应具备的分布式知识

主流分布式架构设计详解

架构开发基础

多线程开发

高性能NIO框架

架构核心服务层技术

服务的前世今生

深入理解通讯协议

基于分布式RPC解决方案

Dubbo全解析

架构关键基础设施

分布式环境指挥官Zookeeper

分布式消息通讯异步与MQ

分布式缓存

数据存储SQL&NoSQL

高冰分流技术Nginx

分布式架构实战

分布式解决方案

Session跨域共享实战

分布式事务解决方案实战

分布式锁解决方案实战

分布式单点登录实战SSO

分布式调度任务系统

分布式配置中心
