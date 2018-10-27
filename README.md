# Spring-Notes
Spring源码学习笔记，从基本的使用出发，剖析功能底层实现方式


# 前言
主要以功能罗列的方式对源码进行学习，以下涉及到的Spring模块：
- Spring IOC/DI
- Spring MVC
- Spring AOP
- Spring Boot  
针对每个模块中的一些功能，进行针对性的研究。

# 一、Spring MVC
- Controller方法参数绑定  
场景：想对传入Controller中的方法的传入参数进行修改  
疑问：Controller中的方法的传入参数如何被赋值的？怎么根据注解@RequestParam、@RequestBody将值赋给指定类型的参数？自定义参数HandlerMethodArgumentResolver是怎么实现的？切面环绕增强修改参数是怎么实现的？这两者有什么差别，如果都实现了，谁先谁后执行？  
- DispachterServlert执行流程 
# 二、Spring IOC/DI
- Bean生命周期  
- IOC和DI流程
- 如何控制单例和多例
# 三、Spring AOP
- cglib和jdk动态代理实现AOP的具体流程
- 哪种情况下选择哪种代理模式，Spring是怎么控制选择哪种代理模式的？
- 拦截器实现原理
- Spring事务实现原理
# 四、Spring Boot
- Bean自动装配策略
- 默认包扫描
- 内置Tomcat原理
- @springbootapplication 注解原理
- @Configuration和@Bean


