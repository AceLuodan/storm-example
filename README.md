# storm + kafka + hdfs

storm 0.9.6

kafka_2.10 0.8.2.2

涉及到的内容:

    kafka + spring
    storm + kafka
    storm + hdfs
    kafka + storm +hdfs

storm WordCountTopology集群环境运行方式

```bash
storm jar net.aimeizi.example.storm.WordCountTopology s1
```


storm + kafka 集群环境搭建

拷贝kafka安装目录下lib目录下的jar到storm集群目录下的lib目录。具体拷贝清单文件如下:


```
kafka_2.10-0.8.2.2.jar
kafka-clients-0.8.2.2.jar
metrics-core-2.2.0.jar
scala-library-2.10.4.jar
snappy-java-1.1.1.7.jar
zkclient-0.3.jar
zookeeper-3.4.6.jar
storm-kafka-0.9.6.jar
guava-11.0.2.jar
curator-framework-2.5.0.jar
curator-client-2.5.0.jar
log4j-1.2.16.jar
jopt-simple-3.2.jar
```


storm kafka集群测试环境运行

```bash
storm jar net.aimeizi.example.MyKafkaTopology s1
```

# 参考文章

https://github.com/spring-projects/spring-integration-kafka

https://github.com/smallnest/spring-kafka-demo

http://shiyanjun.cn/archives/934.html

http://blog.csdn.net/weijonathan/article/details/18301321