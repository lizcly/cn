# 核心概念

## 1. 消息相关名词 
| 术语名称 | 对应英文 | 解释 |
| :- | :- | :- |
| 消息 | Message | 消息队列中数据传输的载体 |
| 消息ID | Message ID | 消息的全局唯一标识，由系统自动生成，唯一标识某条消息 |
| 消息主体 | Message Body | 消息所承载的消息内容，也就是所要传送的数据 |
| 标签 | Tag | 消息队列 JCQ允许对订阅者和消息设置tag来进行消息过滤，确保订阅者最终只消费到他想获得的消息。tag是消息订阅者对于消息的筛选，当订阅者设置了tag时，有相同tag的消息才能被订阅者消费，如果没有设置tag，则订阅者对消息不做筛选。单个订阅者可最多可添加5个标签，单个标签为不超过64个字符的字符串，以‘,’号分割 |
| 消息生命周期 | Message Lifecycle | 消息存在服务端最长的存活时间，从消息成功写入开始计算，不论消息是否被消费过都将被删除，单位为秒，默认值为259200（3天），不允许修改 |
| 消息最大长度 | Maxium Size | 限制消息主体的大小最大为256KB |
| 延时消息 | Delayed Message | 消息的生产者发送一条消息到服务端但是并不想这条消息马上被投递，而是延迟设定的一段时间后才投递给消费者进行消费，该类消息被称为延时消息 |
| 顺序消息 | Ordered Message | 消息队列 JCQ提供的一种严格按照顺序进行发布和消费的消息类型。顺序消息由两个部分组成：顺序发布和顺序消费 |

## 2. 主题订阅相关名词 
| 术语名称 | 对应英文 | 解释 |
| :- | :- | :- |
| 主题 | Topic | 通过创建topic来对消息进行消息分类 |
| 订阅者 | Subscriber | 消息服务的订阅者 |
| 主题 | Topic | 通过创建topic来对消息进行消息分类 |
| 消费组 | ConsumerGroup |  |

## 2. 其他相关名词 
| 术语名称 | 对应英文 | 解释 |
| :- | :- | :- |
| 消息堆积 |  |  |
| 消息过滤 |  |  |
| 重置消费位点 |  |  |


