###### **本demo是针对产品、设备上行sdk方法介绍(即：quecloud-sdk-standard-msg jar的介绍)**
# 开发环境
- JDK1.8
- maven 3.6.3

# 设备上行方法介绍
- 1.QueCloudDevUplinkDemo.java中有设备上行(即:从rabbitmq接收数据)调用过程及参数说明
- 2.更改AccessKey、AccessSecret、connectionUrl(连接地址)、queueName(队列名称)
- 3.实现HandleMessage接口

## 多租户
针对需要同时监听不同的队列,根据AccessKey、AccessSecret、connectionUrl、queueName创建不同AmqpClient对象即可
