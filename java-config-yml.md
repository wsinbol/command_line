# 数据库普通配置方式

```
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/cancreate?useUnicode=true&characterEncoding=utf-8&autoReconnect=true&zeroDateTimeBehavior=convertToNull&allowMultiQueries=true&useSSL=false
    username: root
    password: rootroot
    driver-class-name: com.mysql.cj.jdbc.Driver
```


# 数据库连接池配置方式

```
// 连接池配置方式
spring:
  datasource:
    type: com.alibaba.druid.pool.DruidDataSource
    driver-class-name: com.mysql.jdbc.Driver
    url: jdbc:mysql://localhost:3306/app_com?useUnicode=true&characterEncoding=utf8
    username: root
    password: rootroot
    druid:
      #2.连接池配置
      #初始化连接池的连接数量 大小，最小，最大
      initial-size: 5
      min-idle: 5
      max-active: 20
      #配置获取连接等待超时的时间
      max-wait: 60000
      #配置间隔多久才进行一次检测，检测需要关闭的空闲连接，单位是毫秒
      time-between-eviction-runs-millis: 60000
      # 配置一个连接在池中最小生存的时间，单位是毫秒
      min-evictable-idle-time-millis: 30000
```

