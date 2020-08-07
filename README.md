# RespConnection
通过RESP协议跟Redis服务器交互

用法：
```java
RespConnection connection = new RespConnection("localhost", 6379);
// 向服务器发送指令
connection.send("set", "foo", "apple");
// 从服务器获取返回值
RespType result = connection.receive();
```
