# SpringCloudDemo

## 已实现功能
- 日志

- 集成Job

- 集成druid数据库

- 集成ES（未验证）

- 增加MapStruct对象转换工具
```text
1.新建具体转换规则类UserMapper-必须
2.新建特殊转换逻辑HandWritten-非必须

注意事项
    pom.xml中需要增加相关包和插件

```


## 踩坑

#### 多数据源导致事务失败
```text
配置多个数据源后，代码中事务事务时，需要指定事务管理器名称，否则使用名称为transationManager的事务管理器，会导致事务不生效
```