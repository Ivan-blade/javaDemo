# javaDemo

### 简述

+ 项目大小（complete > part > demo）

### Demo-JDBC简单使用

  + 使用通过QueryRunner以及DataSource连接池操作数据库
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage2-Module2/">solution</a>

### Part-前端三板斧（html+css+js）简单使用
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage3-Module1/">task02+配合demo.mp4使用</a>
### Part-前端jquery+bootstrap简单使用
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage3-Module2/">solution</a>
### Part-servlet+jsp+jdbc mvc架构使用
  + 任务：要求使用管理员账号密码 登录后进行学员信息增加、学员信息修改、学员信息删除、学员信息查找、学员信息显示功能。 
  + 整个业务分为
    + bean层
      + 存放javabean对象
    + dao层
      + 用于结合jdbc编写sql语句
    + factory层
      + 用于返回dao层对象，在传统的岁月里，还没有spring的控制反转的特性，暂且用工厂类替代spring生成对象
    + service层
      + 用于编写具体逻辑
    + serlvet层
      + 编写接口
    + 前端webapp
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage4-Module1/Stage4-Module1/src/com/lagou/demo03">solution</a>
### Part-EL 表达式、过滤器的简单使用
  + 任务：使用 Cookie 实现一周内免登录在mvc项目的基础上继续扩展其他功能
  + 在mvc的基础上增加了filter层，其中的**LoginFilter**继承filter接口对访问进行校验，如果客户端浏览器的cookie对象中没有username对象，则将页面转发到登录界面，如果存在username对象则将该对象保存到session中放行该访问
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage4-Module2/design.md">更详细设计</a>
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage4-Module2/">solution配合目录中的demo.mp4使用</a>
### Part-mvvm架构后端demo
  + 任务：编写后端程序
    + 在mvvm架构中后端只负责提供接口用于返回前端所需要的数据
  + 功能实现：
    + 常见增删查改功能，文件上传功能编写
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage5-Module1/">solution</a>
### Demo-Mybatis简单使用
  + 传统的jdbc操作有些复杂，包括sql语句的硬编码问题以及获取结果时的处理都不是很简便，mybatis应运而生
  + 任务使用基于xml的mybatis进行常crud操作
  + 业务结构
    + Java
      + domain
        + 存放javaBean
      + mapper
        + mapper接口
      + test
        + 测试mapper方法
    + Resources
      + mapper
        + 编写具体的sql语句
      + jdbc.properties
        + jdbc配置数据源信息
      + sqlMapConfig.xml
        + myBatis配置文件
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module1/">solution</a>
### Part-spring+jdbcTempate
  + 简单使用spring的IOC和AOP
  + 业务结构
    + java
      + advice
        + 存放通知方法
      + dao
        + 结合jdbcTemplate编写sql语句
      + domain
        + 存放javaBean
      + service
        + 编写业务逻辑
      + Test
        + 结合JUnit4对dao层中的方法进行单元测试
    + resources
      + ApplicationContext.xml
        + spring的配置文件，规定了扫描注解的范围，配置了需要进行控制反转的类（该项目中包括jdbcTempate，dao和service类）以及需要进行切面处理的规则
      + Jdbc.properties
        + jdbc数据源配置
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module2/">solution</a>

### Part-spring+springmvc+mybatis
  + 任务：使用上述框架实现crud
  + 业务结构
    + java
      + controller
        + 设计接口以及相应功能
      + dao
        + 定义接口
      + domain
        + 存放javaBean
      + service
        + 编写业务逻辑
      + test
        + junit单元测试service功能
    + resources
      + dao
        + sql语句编写
      + ApplicationContext.xml
        + spring配置
      + Spring-mvc.xml
        + spring-mvc配置
      + Jdbc.properties
        + jdbc配置
  + <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module3/">solution</a>
### 多模块ssm后端编写
  + 任务：使用多模块设计ssm后端crud
  + 业务结构
    + dao模块
      + 依赖domain模块
    + domain模块
    + service模块
      + 依赖dao模块
    + utils模块
    + web模块
      + 依赖service模块
  + <a src="https://gitee.com/ivanblade/lagou-homework/tree/Stage6-Module4/">solution</a>

### complete-dubbo+zookeeper+mysql+spring+springMVC+mybatis

+ 使用如上技术栈完成crud（别问为什么全是crud）
+ 业务结构
  + dao
    + 编写sql
  + entity
    + javaBean
  + interface
    + 编写service接口
  + service
    + 实现service接口
  + web
    + 编写接口调用service方法
  + zookeeper部署在虚拟机中

### part-fastdfs分布式文件系统使用

+ 完成文件上传功能，将文件上传到fastdfs服务器中
  + fastdfs部署在虚拟机中
  + 前端采用vue+element（事实上只用了一个文件上传组件...）
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage7-Module2">solution</a>

### compelete-springcloud简单使用

+ 技术栈：springboot+springcloud(gateway+eureka+Config+Bus+feign)+nginx+mybatis-plus

+ 业务结构
  + lagou-parent：父微服务，所有微服务继承
  + lagou-cloud-gateway：网关微服务，集群环境，端口号分别为：9000、9001
  + lagou-service-order：订单微服务，集群环境，端口号分别为：9100、9101
  + lagou-service-goods：商品微服务，商品微服务，集群环境，端口号为别为：9200、9201
  + laoug-service-common：公共组件微服务，放置所有业务微服务的POJO和Feign接口
  + lagou-cloud-eureka：服务注册与发现微服务，集群环境，端口号分别为9300、9301
  + lagou-cloud-config：配置管理微服务，非集群环境，端口号9400
  + 最后Nginx实现对gateway的负载均衡
+ 实现功能
  + 实现微服务的高可用（每个微服务都会进行负载均衡）
  + 设置熔断服务以及服务降级方法
+ <a href="https://gitee.com/ivanblade/lagou-homework/blob/Stage9-Module1/%E8%AE%BE%E8%AE%A1%E6%80%9D%E8%B7%AF.md">其他细节</a>
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage9-Module1/">solution</a>

### part-mysql分库分表操作

+ 技术栈：springboot+shardingsphere+mybatis+mysql（此外还可以使用mycat做一定配置之后就可以操作最后的一张逻辑表，mycat自动对物理表进行分库分表操作）

+ 任务：对数据库进行分库分表后进行crud操作
+ 实现功能：
  + 数据库：lg_novel_db，lg_user_db，lg_region_db
  + novel和user属于不同业务范畴数据不放在一个数据库中，进行垂直分库（就是分别放在两个数据库里）
  + region表作为公共表, 冗余在 两个库中
  + 对novel表 进行读写分离,创建主库与从库.（需要在mysql提前在mysql中做主从配置）
  + 对users表进行水平分表,分片键使用户id, 分片策略为id%2+1
  + 最终效果
    + lg_novel_db(主库)——部署在虚拟机中（172.16.161.140）
    + lg_novel_db(从库)——部署在虚拟机中（172.16.161.138）
    + lg_user_db（172.16.161.140）
      + Users_1
      + Users_2
    + lg_region_db
+ <a href="https://gitee.com/ivanblade/lagou-homework/blob/Stage9-Module3/code/process.md">其他细节</a>
+ <a href="https://gitee.com/ivanblade/lagou-homework/tree/Stage9-Module3/">solution</a>

### Compelete-个人项目：遗传算法解决tsp问题（大二暑假，19年8月）

+ 主要功能：返回多个地点之间的最佳路线
+ 技术栈：servlet+jsp（数据源采用了高德api和百度api）
+ 感受：当时也是老师让做的，就是网上找一个遗传算法样本，然后看懂了自己改成和自己能用的，隐约记得代码比较丑陋，当时第一次接触web开发，原先是只改了算法，然后数据源是使用的excel文件，然后老师让用界面显示出来，开始了解web，于是误入servlet+jsp加tomcat，对于接口的使用比较复古，使用的截取字符串的方式，一开始只写了百度api获取，后来同项目组的同学好像用高德api不太会用，然后我顺便写了获取高德api的方法两个人一起用了，最近毕设用到了，一启动发现高德api跑不了了，还好百度还没挂
+ <a href="https://github.com/Ivan-blade/GA_to_tsp_baidu_api">solution</a>

### Complete-个人项目：比较粗糙的前后端分离项目(好像是大三上学期写的，19年10月)

+ 主要功能：crud
+ 技术栈：vue+springboot+mybatis

+ <a href="https://github.com/Ivan-blade/springboot-vue">solution</a>
+ 感受：当时是刚开始学开发，项目导向，老师让模仿运满满的app，直接网上学了springboot和vue就上了，而且vue没有用ui框架，手写的前端ui部分ui面向百度，后端也比较简单，各种意义上都比较粗糙，除了简单的crud其他就没了

### complete-个人项目：可匹配日记应用(2020-3月)

+ 主要功能：写日记，还可以匹配其他人
+ 技术栈：vue+vuetify+springboot+mybatis+springsecurity
+ <a href="https://github.com/Ivan-blade/tell_you_other_day">solution</a>
+ 感受：那时候想自己做点东西，于是就上了，前端使用了ui框架（事实证明设计能力不到位给了ui框架做出来的前端依然不太能打），后端引入了security，不过只是轻度使用，只有登录时用了一下登录处理的url，对于权限控制并没有使用太多，当时好像想使用多模块思想开发这个项目来着，但是网上的视频讲的不是很清楚，然后就比较诡异了，项目使用hbuilder打包成了app然后后端部署到了阿里云，目前还在跑（2021-3-5），后来就开始参加系统培训了，对于很多东西都有了更深入的了解

