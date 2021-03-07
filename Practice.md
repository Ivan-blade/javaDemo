### java基础

+ 题目：实现双色球抽奖游戏中奖号码的生成，中奖号码由 6 个红球号码和 1 个蓝球号码组成。 其中红球号码要求随机生成 6 个 1~33 之间不重复的随机号码。 其中蓝球号码要求随机生成 1 个 1~16 之间的随机号码。 

  + 考点：Random类使用，Arrays工具类使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/blob/Stage1-Module1/homework/test3.md">solution</a>

+ 题目： 实现数组扩容。自定义数组长度（用户指定），扩容规则：当已存储元素数量达到总容量的 80%时，扩容到原容量的1.5 倍。 例如，原容量是 10，当输入第 8 个元素时，数组进行扩容，容量从 10 变 15。

  + 考点：数组的基础使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/blob/Stage1-Module1/homework/test4.md">solution</a>

+ 题目:编程实现控制台版并支持两人对战的五子棋游戏，棋盘用二维数据表示

  + 考点：二维数据以及五子棋规则的实现
  + <a href="https://github.com/Ivan-blade/lagou-homework/tree/Stage1-Module2/homework/backgammon/src/com/Ivan/homework1">solution</a>

+ 题目： 编程统计字符串"ABCD123!@#$%ab"中大写字母、小写字母、数字、其它字符的个数并打印出来。

  + 考点：Character工具类的使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/blob/Stage1-Module3/homework/Stage1-Module3/src/com/Ivan/task01/TestMain.java">solution</a>

+ 题目： 准备一个 HashMap 集合，统计字符串"123,456,789,123,456"中每个数字字符串出现的次数并打印出来。

  + 考点：hashmap的简单使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/blob/Stage1-Module3/homework/Stage1-Module3/src/com/Ivan/task03/TestMain.java">solution</a>

+ 题目： 使用集合实现斗地主游戏的部分功能，要求如下： 

   （1）首先准备 54 张扑克牌并打乱顺序。 

   （2）由三个玩家交替摸牌，每人 17 张扑克牌，最后三张留作底牌。 

   （3）查看三个玩家手中的扑克牌和底牌。 

   （4）其中玩家手中的扑克牌需要按照大小顺序打印，规则如下： 

    手中扑克牌从大到小的摆放顺序：大王,小王,2,A,K,Q,J,10,9,8,7,6,5,4,3

  + 考点Collection工具类使用，list，treeset，比较器的使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/tree/Stage1-Module3/homework/Stage1-Module3/src/com/Ivan">solution</a>

+ 题目：a.使用 List 集合实现简易的学生信息管理系统，要求打印字符界面提示用户选择相应的功 能，根据用户输入的选择去实现增加、删除、修改、查找以及遍历所有学生信息的功能。

    b.自定义学号异常类和年龄异常类，并在该成员变量不合理时产生异常对象并抛出。 

    c.当系统退出时将 List 集合中所有学生信息写入到文件中，当系统启动时读取文件中所 有学生信息到 List 集合中。 

  + 考点：list集合使用，ObjectInput/OutputStream使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/tree/Stage1-Module4/lagou-homework/Stage1-Module4/src/com/Ivan/task01">solution</a>

+ 题目：使用基于 tcp 协议的编程模型实现多人同时在线聊天，要求每个客户端将发 送的聊天内容发送到服务器，服务器接收到后转发给当前所有在线的客户端。

  + 考点：socket编程，文件传输，多线程使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/tree/Stage1-Module4/lagou-homework/Stage1-Module4/src/com/Ivan/task05">solution</a>
  + 这边好像是线程嵌套线程。。。很不优雅，有机会改一下

+ 题目：  a. 使用线程池将一个目录中的所有内容拷贝到另外一个目录中，包含子目录中的内容。

    b.实现将指定目录中的所有内容删除，包含子目录中的内容都要全部删除。 

  +  考点：File类简单使用
  + <a href="https://github.com/Ivan-blade/lagou-homework/blob/Stage1-Module4/lagou-homework/Stage1-Module4/src/com/Ivan/task02/Test.java">solution</a>

### 未完成项目

+ 拉勾教育ssm后端
  + 多模块架构
    + ssm-dao
    + Ssm-domain
    + ssm-service
    + ssm-util
    + ssm-web
  + 功能分布
    + 课程管理
    + 用户管理
    + 权限管理
    + 广告管理
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module4/">solution</a>

### 拉勾教育ssm前端

+ vue前端
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module5/">solution</a>

### RabbitMQ

### 分布式拉勾前后端

+ 后端
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage8-Module1/">solution</a>
+ 前端
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage8-Module2/">solution</a>

### Elasticseach+kafka+docker

+ 简单使用如上工具
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage9-Module2/">solution</a>

### 拉勾微服务前后端分离

+ 如题
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage9-Module2/">solution</a>

