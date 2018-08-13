# 创建核心

### 使用create命令

```
./Solr create -c solr_core_name #创建一个名为solr_core_name的核心
```

Solr可以创建多个核心，使用页面上的核心选择器选择核心

### 使用create\_core命令

```
#创建一个名为core_name的核心，可以通过-p参数指定端口，-d参数指定端口的配置目录
./Solr create_core -c core_name [-p port] [-d conf_dir]
```

# 删除核心

```
./Solr delete -c core_name #删除一个名为core_name的核心
```



