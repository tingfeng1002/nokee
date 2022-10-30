# nokee
Notify memory data storage system of key expiration event  &amp;&amp; key 过期 事件 通知 内存 数据存储系统

## 来源
做iot硬件设备掉线管理时候，使用协议的心跳间隔做为redis的ttl，key 过期事件通知应用程序。
但是通知测试 有时候不触发，排查一圈问题觉得是配置文件中配置项问题，但是其他应用又同时使用该redis,SpringDataRedis 对于集群订阅事件的支持与单机版不一致
使用条件注解切换不同的bean 不是很满足当前现状
