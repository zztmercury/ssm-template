# 使用说明
导入项目后，根据需要修改项目内/src/main/java/目录下的包名，然后修改以下配置文件
- /gradle.properties 配置mybatis generator自动生成代码的存放位置
- /src/main/resources/config/db.properties 数据库连接的配置文件
- /src/main/resources/config/log4j2.xml log4j2的配置文件，主要吧log的输出路径改了即可
- /src/main/resources/config/spring/* 修改配置中的包名即可
- /src/main/resources/config/mybatis/generatorConfig.xml 参考[MyBatis Generator介绍](http://generator.sturgeon.mopaas.com/index.html)进行配置
- /setting.gradle 配置项目名
- /build.gradle 配置所属组织及版本号

修改完成后刷新gradle项目，可以在task->other下面找到mybatisGenerate，运行后即可根据generatorConfig.xml自动生成相应的mapper(DAO)和pojo

springMVC可以参考[跟开涛学SpringMVC](http://jinnianshilongnian.iteye.com/blog/1752171)