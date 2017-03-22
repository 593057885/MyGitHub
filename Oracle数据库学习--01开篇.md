# Oracle数据库学习--01开篇

标签：Oracle数据库

---
## 数据库简介

 - 小型：access、foxbase

> 特点：负载量小，用户大概100人以内（留言板、信息管理系统）;成本在千元内，对安全性要求不高。

 - 中型：sqlserver、mysql

> 特点：负载量，日访问量在5000-10000；成本在万元以内（商务网站）；满足日常安全需求。

 - 大型：sybase、db2、oracle

> 特点：海量负载，可以处理海量数据（sybase<<"oracle"<<"db2"海量处理能力)；安全性高，相对贵。

---
## 一、大纲

 - 概论：发展
 - 关系数据库系统：sql、事务、sql优化、索引。
 - 提高篇：数据库设计，数据安全性，并发控制，数据库管理系统，数据库完整性，数据库恢复技术。
 - 高级篇：存储过程、触发器、游标、函数

---
## 二、DBMS
关系型数据库（database manager system）
常见的DBMS系统：
> 商业：Oracle、SQLServer<br> 开源：MySQL、PgSQL

### 关系操作：

 1. 数据查询：选择 投影 连接 并 交 差
 2. 数据操作：增加 删除 修改 查询
 3. 相关完整性约束包括：
 - 实体完整性
 - 参照完整性
 - 用户定义完整性

---
## 三、SQL语言
定义：SQL(Structured Query Language)
分类：
>  1. DDL:Data Definition Language
>  2. DCL:Data Control Language
>  3. DML:Data Management Language
>  - DQL:Data Query Language 
>  - DML:Data Management Language

命令：

 - DDL:create/drop/alter/rename/truncate(截断)
 - DML:insert/delete/update/select 
 - DCL:grant/revoke/commit/rollback

---
## 四、配置PL/SQL远程连接Oracle

- 1、配置被连接的数据库静态监听（listener.ora）
``` ora	
SID_LIST_LISTENER = 
(SID_LIST = 
    (SID_DESC = 	 
        (GLOBAL_DBNAME=orcl) 	 
        (ORACLE_HOME=D:\app\Administrator\product\11.2.0\dbhome_1) 
        (SID_NAME=orcl) 	
    )   
)
```
```
LISTENER =
  (DESCRIPTION_LIST =
    (DESCRIPTION =
      (ADDRESS = (PROTOCOL = IPC)(KEY = EXTPROC1521))
      (ADDRESS = (PROTOCOL = TCP)(HOST = USER-20161019GF)(PORT = 1521))
    )
  )
```

> ps:要能其他客户端访问，需将listener中host属性设置为本地主机名/对外访问的ip地址

- 2、解压客户端连接工具
E:\libinghua\oracle\tools\PLSQLDeveloper\PLSQL\instantclient_11_2\tnsnames.ora
添加一台数据库连接信息：
```
ORCL =
  (DESCRIPTION =
    (ADDRESS = (PROTOCOL = TCP)(HOST = 127.0.0.1)(PORT = 1521))
    (CONNECT_DATA =
      (SERVER = DEDICATED)
      (SERVICE_NAME = orcl)
    )
  )
```

- 3、将整个instantclient_11_2目录配置到系统环境变量中
```
NLS_LANG = SIMPLIFIED CHINESE_CHINA.ZHS16GBK 
TNS_ADMIN = D:\install\PLSQLDeveloper\PLSQL\instantclient_11_2 
```
- 4、oci.dll文件配置
打开PL/SQLDeveloper工具不登录进入界面。
配置首选项中的连接属性：指定Oracle主目录、oci库文件的位置
