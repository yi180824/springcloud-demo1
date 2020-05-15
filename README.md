# 入门级springcloud搭建
## 概述：使用spirngcloud实现分布式，用来测试微服务
### 已实现功能
    1.实现了基本的功能：注册中心、数据微服务、视图微服务
    2.实现了服务器、客户端的配置
### 待实现功能
	1.服务链路追踪 zipkin
	2.消息总线bus:使用消息队列 RabbitMQ实现
	3.断路器 Hystrix
	4.断路器监控与管理 HystrixDashboard
	5.断路器聚合与监控 turbine（漩涡机）
	6.网关 zuul
### 搭建步骤：
    第一步：创建parentMavenProject父模块
    第二步：创建eureka-server子模块，注册中心 eureka
    第三步：创建product-data-service子模块，数据微服务
    第四步：创建product-view-service-ribbon子模块，视图微服务
    第五步：创建product-view-service-feign子模块，视图微服务（feign是 ribbon的改进，支持使用注解开发，更加方便，以后都用feign）
    上面的是基本开发知识点，以此就可以开发了，下面的是使分布式更加完善
    第六步：创建config-server子模块，配置服务器
    第七步: 创建bootstrap.yml，配置客户端
    第八步：从第二步开始，就可以在对应的界面查看效果了
