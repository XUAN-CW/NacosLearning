---
tags:
- nacos
- mysql
---

# 版本要求

5.6.5+ ，mysql 8 以下

# 创建数据库

 [nacos-mysql.sql](data\nacos-mysql.sql) 

根据下面的信息创建

```
spring.datasource.platform=mysql
db.num=1
db.url.0=jdbc:mysql://127.0.0.1:3306/nacos_config?
characterEncoding=utf8&connectTimeout=1000&socketTimeout=3000&autoReconnect=true
db.user=root
db.password=root
```

# 配置 nacos

编辑 `nacos/conf/application.properties` ，在最后加上：

```
spring.datasource.platform=mysql
db.num=1
db.url.0=jdbc:mysql://127.0.0.1:3306/nacos_config?
characterEncoding=utf8&connectTimeout=1000&socketTimeout=3000&autoReconnect=true
db.user=root
db.password=root
```









