# Spring Cloud 实践学习案例

> 转载请标明出处：https://windmt.com/tags/Spring-Cloud/ 本文出自 [Yibo's blog](https://windmt.com)

Spring Cloud 实践学习案例，由浅入深一步一步学习 Spring Cloud，是 Spring Cloud 初学者及核心技术巩固的最佳实践。

本示例代码采用 Spring Boot 2.1.0.RELEASE，Spring Cloud 版本为 Finchley.SR2。

## Eureka Server

服务注册几乎每次都要用到，为了方便我做了一个 Dockerfile。
使用以下命令可以直接拉取使用镜像：

```shell script
docker pull haoyizebo/eureak-server
docker run --name=eureka-server -p 8761:8761 -t haoyizebo/eureka-server
```

查看 log

```shell script
docker container logs -f eureka-server
```
