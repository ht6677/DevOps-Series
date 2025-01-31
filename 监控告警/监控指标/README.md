# 监控系统指标

# 监控的对象和指标

监控已然成为了整个产品生命周期非常重要的一环，运维关注硬件和基础监控，研发关注各类中间件和应用层的监控，产品关注核心业务指标的监控。可见，监控的对象已经越来越立体化。

## 硬件监控

包括：电源状态、CPU 状态、机器温度、风扇状态、物理磁盘、raid 状态、内存状态、网卡状态。

## 服务器基础监控

- CPU：单个 CPU 以及整体的使用情况
- 内存：已用内存、可用内存
- 磁盘：磁盘使用率、磁盘读写的吞吐量
- 网络：出口流量、入口流量、TCP 连接状态

## 数据库监控

包括：数据库连接数、QPS、TPS、并行处理的会话数、缓存命中率、主从延时、锁状态、慢查询

## 中间件监控

- Nginx：活跃连接数、等待连接数、丢弃连接数、请求量、耗时、5XX 错误率
- Tomcat：最大线程数、当前线程数、请求量、耗时、错误量、堆内存使用情况、GC 次数和耗时
- 缓存 ：成功连接数、阻塞连接数、已使用内存、内存碎片率、请求量、耗时、缓存命中率
- 消息队列：连接数、队列数、生产速率、消费速率、消息堆积量

## 应用监控

- HTTP 接口：URL 存活、请求量、耗时、异常量
- RPC 接口：请求量、耗时、超时量、拒绝量
- JVM ：GC 次数、GC 耗时、各个内存区域的大小、当前线程数、死锁线程数
- 线程池：活跃线程数、任务队列大小、任务执行耗时、拒绝任务数
- 连接池：总连接数、活跃连接数
- 日志监控：访问日志、错误日志
- 业务指标：视业务来定，比如 PV、订单量等
