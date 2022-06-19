- spring boot没有配置数据库，导致启动报错
  - pom.[xml](https://so.csdn.net/so/search?q=xml&spm=1001.2101.3001.7020)中导入了jbdc和mybatis的jar包依赖。但是application.yml（或aoolication.properties）文件中没有配置数据库，导致的启动失败
  - spring boot默认会加载org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration
    类，DataSourceAutoConfiguration类使用了@Configuration注解向spring注入了dataSource bean。因为工程中没有关于dataSource相关的配置信息，当spring创建dataSource bean因缺少相关的信息就会报错。
  - 查看是否还配置了其他的依赖。比如[mybatis](https://so.csdn.net/so/search?q=mybatis&spm=1001.2101.3001.7020)，druid数据库链接池。
  - 终极代码：@SpringBootApplication(exclude={DataSourceAutoConfiguration.class, MybatisAutoConfiguration.class, DruidDataSourceAutoConfigure.class})