# chess
在线五子棋

---

技术栈：  HTML +canvas（前端绘图插件）+WebSocket（全双工通信协议）+Gson（序列化工具）

项目需求：

1. 对手配对，房间分配：利用匹配队列BlockingQueue和ConcurrentHashMap分配对手,并用uuid生成一个房间号
> 遇见问题：高并发问题 			

>解决方式：采用生产者消费者模式来进行“削峰”
2. 下棋者落子，结果分析：通过一个单例实现的房间管理者来进行操作

项目源码：https://github.com/hello413/chess      演示地址：http://itpainter.xn--ses554g:8080/chess/