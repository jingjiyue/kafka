1.消息队列的作用:
  1).解耦
  2).冗余
  3).扩展性
  4).灵活性&峰值处理能力
  5).可恢复性
  6).顺序行
  7).缓冲
  8).异步通信
2.工作模式
  1).点对点模式:一对一,由消费者主动拉取数据,消息收到后清除队列
  2).发布/订阅模式:一对多,数据产生后由队列推送给订阅者
3.kafka是一个分布式消息队列:
  1).对消息保存是根据topic进行归类的
  2).每个kafka实例成为broker
  3).kafka集群和consumer都依赖于zookeeper保存的meta信息
  4).同一个消费组的消费者不能消费同一个topic分区的数据
