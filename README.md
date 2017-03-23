# MyGitHub
临时存放
.LOG

## 毕业设计题目是B/S模式下的办公家具企业连锁店管理系统的设计与实现

---
![背景图片](https://github.com/593057885/MyGitHub/blob/master/idream.jpg?raw=true)
### 到现在为止已经完成的工作有

1.需求分析：系统用户有哪些，系统有哪些模块，每个模块有哪些功能

2.数据库设计：先分析系统中有哪些实体，然后制作出系统的总E-R图，在写出各个实体的分E-R图，用VISIO画的图

3.详细设计：
  3.1页面设计：用VISIO将每个模块用到的页面的大致布局画出来，方便页面制作页面采用JSP技术制作
  3.2后台设计：根据E-R图创建表字段，创建表间关联约束（主键，外键，非空，检查约束等等）

4.编码任务：
  4.1前台页面编码：
  4.2后台编码：
     系统搭建：采用当前软件行业比较流行的JavaWeb技术，运用MVC分层设计思想，使用Hibernate+Spring+SpringMVC来搭建环境,设计实体类（entity）、数据库访问类（dao）、服务类（service）、控制层类（web/controller）配置web.xml、spring.xml、spring-hibernate.xml、spring-mvc.xml，创建conf.properties文件存储数据库连接字段，配置ehcache.xml优化系统响应时间。

8:43 2016-12-26

系统开发使用的工具是MyEclipse2014，数据库是MySQL

心得：要想写好后台，需要对前台比较熟悉，特别是Ajax传输数据这部分，对于表格的操作，以及编写个性化对话框，使用ExtJS能达到更好的效果，对于前台事件响应的话使用JQuery来做会省事很多，注重写单元测试类，来及时验证功能的完整性

8:53 2016-12-30

SpringMVC的使用：配置SpringMVC拦截器（servlet）时，不需要拦截所有请求，在url-parttern中*.do的写法更好，表示只拦截*.do结尾的URI，程序编写时更加灵活

19:03 2017-1-3

张传波：UML类图与需求分析的大战：类图、活动图、用例图、顺序图、状态机图

23:09 2017-1-4

今天非常的傻
火车票本来可以改签的，但是没有立即改签，回来后才改签发现时间刚好不够了，只能自己哭了，办事情没有个重要性的概念，自己不够抓紧时间，需要学习番茄时间管理

21:31 2017-1-5

图书馆学习：今天看的书单
1.eclipse开发技术详解：这本书，大致明白eclipse是使用什么技术开发出来的
2.QT5实战开发：开发C++程序
3.GOF设计模式
4.Git和GitHub区别（CVS、Subversion）
5.软件开发项目管理
6.Maven使用
7.Delphi开发

15:21 2017-1-6

QT工作原理：
信号量和槽机制：类型安全，松散耦合
QT元对象系统：
布局管理器：

13:13 2017-1-7

今天就要回家了，又是忙碌的一天，我的心情很乱，对未来的不确定因素充满了畏惧心理，回家学一些编程方面的技术，期待再2017年能够找份好工作，为家里减轻负担

19:34 2017-1-9

回家两天的感受：
8号回家，下火车，坐上回汝城文明的班车，50分钟到了，体会到了，修县级高速公路的便利
听说大姑父患有轻度冠心病，提醒他注意身体
回家就碾米了，体会家中农村生活的不易，送弟弟妹妹去学校，分析零花钱的消费
9号打扫，整理家务，家中物件的分门别类存放不是一件简单的事情，但是做好了用处很大

0:24 2017-1-11
问题记录：
在使用SpringMVC和FreeMarker时，当类上有RequestMapping字段是，采用转发的形式，html页面上以相对路径定位的资源会丢失，如何解决呢？FreeMarker对空值的情况如何处理？

23:07 2017-1-28
Mybatis的使用：
Mybatis-config.xml
ObjectMapper.xml
select,insert,update,delete,resuletMap,sql,parameterType,resultMap

13:32 2017-1-30
coffer（中国人民银行web版）源码阅读分析：
persistence层：持久层（entity + dao）
使用Java类继承的思路精简代码：
entity：创建BeanEntity，DataEntity，业务实体类

0:42 2017-1-31
Hibernate复习：
hibernate.cfg.xml/Entity.hbm.xml
1、组件映射
2、ORM框架了解
3、Hibernate详解：Configuration,SessionFactory,Session,Transaction,Query
4、Hibernate4日志及配置文件
（log4j.properties + Slf4japi.jar + slf4j-log4j.jar + log4j.jar）
5、对象生命周期及crud操作
6、组合主键映射
7、大对象映射

19:31 2017-1-31
北京、上海、深圳、广州、杭州
Java学习详略得当

20:04 2017-2-3
hibernate复习：
Blob blob = new SerialBlob("ttt".getBytes());
Clob clob = new SerialClob("sss".toCharArray());
stu.setImage(blob);
stu.setIntroduce(clob);
12:37 2017-2-7

20:27 2017-2-7
学习新的东西：最好先写helloworld程序，对于到的东西，根据doc文档，一点点往里面加东西，
学习会很快，也很扎实

17:46 2017-2-11
想象学习法，想象面试过程，对面试过程越熟悉，面试的时候越放松，越能发挥出水平
17:49 2017-2-11

面试成功：简历+笔试+沟通+毅力+一点点运气
面试技巧：踏实+忠诚+积极+毅力
薪资价位：由简历+面试发挥决定
踏实，忠诚，积极，胜任
17:53 2017-2-11
沟通原则：不卑不亢，双赢思维，不怕吃苦，不怕吃亏，带齐纸笔，举例画图，展现自己，不成不归
项目经理：关注点比较高，需求，设计，分析
22:15 2017-2-11
面试技巧：

11:27 2017-2-12
笔试题积累：
程序题：规范化，变化写到配置文件中
简答题：简述MVC思想，举例加画图
杂碎知识点，编写配置文件题，能背则背，不能背做小抄
算法题，写思路

面试：围绕项目来问，熟悉项目业务流程，运用沟通技巧

11:33 2017-2-12
自学能力的培养：比如自学log4j
通过网络Google学习，掌握关键字搜索的技巧 ""
大目标分解成小目标
14:07 2017-2-12
faq常见问题合集

1:52 2017-2-13
系统设计：界面原型
需求条目化
数据库表
设计模式设计（系统架构设计）
11:56 2017-2-13
struts-sprng-plugins.jar详解：
交给spring托管后，默认是按照name进行属性注入，改成type后，service层的注解可以不写了，因为是按照类型注入

解决Hibernate的Session关闭问题，spring插件中OpenSessionInView延迟session到Jsp访问完后在关闭
解决OenpSessionInView中SessionFactory实例名不是sessionFactory的情况:

web.xml配置时，filter配置时有先后顺序的
中文乱码解决：可以在struts.xml中配置常量constant，也可以在web.xml配置spring字符过滤器
mysql命令行查看：
show create table user;
set names gbk;
20:07 2017-2-13
简历star法则：situation、task、action、result
在你的工作单位，担任职务下，列出你所干过的事情，在模块Action和Result中以简洁的语言写上
写上实现手段
20:47 2017-2-13

项目介绍：

本系统采用的是J2EE典型的三层结构： 第一层：用户层，即运行在客户端机器上的客户层组件 第二层：功能层：1.action层（运行在J2EE服务器上的Web层组件） 2.server层（运行在J2EE服务器上的业务逻辑层组件） 第三层：数据层，即运行在数据服务器上的DB系统 层次间的依赖关系自下到上。采用的技术有Struts，Spring，Hibernate，Log4J等。其中表现层采用Struts框架开发；业务层封装业务流程，为适应业务的变更，每一业务模块均有专门的接口及实现类，利用Spring的IoC功能将实现类注入给表现层的Action；数据访问层借助于Hibernate实现，代码简洁且可适应不同的数据库。事务部分利用Spring的声明式事务管理。

本项目采用B/S架构，MVC模式，基于struts，hibernate，spring框架来实现，本项目结构上分为表现层、业务层和数据访问层，层间的依赖关系从下到上。其中表现层采用Struts框架开发；业务层封装业务流程，每一业务模块都有专门的接口及实现类，利用Spring的Ioc功能实现依赖注入；数据访问层借用Hibernate实现，代码简洁可以适用不同的数据库。

系统是基于网络BS架构借款系统。系统采用基于J2EE框架相关技术实现,所采用技术全部为当前主流并且成熟框架。系统采用MVC设计模式，AJAX + WEB三层架构 Struts + Spring + Hibernate。利用AJAX提高用户体验。系统表现层采用JSP + Struts，业务模型层采用Spring + JavaBeans ，数据操作层采用Hibernate。

系统采用SSH集成的方式，划分为显示层、Action层、Service层、Dao层四层，使用Hibernate作为数据对象持久化引擎，SpringIOC实现业务对象管理,Struts负责请求的转发和视图管理，这样提高了系统的可维护性、和可扩展性。通过Ajax异步传输机制完成数据无刷新展示，具有更好的用户体验

职责：(1) 参与编码分析及部分文档的编写 (2) 在该项目中主要负责还款管理模块的实现

简述系统背景和架构，自己负责什么，遇到问题如何解决，收获总结，
国内开发特点：独立负责模块开发

23:25 2017-2-14
这两天一直在整理个人简历，体会到网投的不容易呀，如何在几百几千份简历中脱颖而出成了获取宝贵面试机会的关键
13:23 2017-2-15

Java技术自学经验总结：拿到技术，先运行一个标准的HelloWorld程序，在理解程序的基础上看官方说明doc文档，对于每一个细节，运行一个小demo来学习，想要学的深，一定要看英文文档，最新的技术往往是先出英文文档的。根据学习目的来学习知识，一般来说学习到入门就行了，等用到了再去学精

17:51 2017-2-16
毕设论文模块：
需求描述文档
系统给分析与设计
数据库设计
开发接口API docs & 源代码注释
用户帮助（前台）
管理员手册（后台）
测试文档

0:08 2017-2-18
eclipse egit使用从GitHub获取项目
maven jar包下载缓慢，在set.xml中改镜像下载地址为阿里云的mirror（镜像）
11:28 2017-2-18

来上海尚学堂培训，让我想到了很多，人只有努力了才有要求幸福的权利
