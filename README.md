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
  - 场景：想对传入Controller中的方法的传入参数进行修改  
  - 问题：
    1. Controller中的方法的传入参数如何被赋值的？
    2. 怎么根据注解@RequestParam、@RequestBody、@PathVariable将值赋给指定类型的参数？
    3. 自定义参数HandlerMethodArgumentResolver是怎么实现的？
    4. 切面环绕增强修改参数是怎么实现的？
    5. 这两种修改参数的方式有什么差别，如果都实现了，谁先谁后执行？  
- DispatcherServlet执行流程 
- 返回ModelAndView的策略（json、xml、模板引擎、字符串）
- @Controller、@RequestMapping初始化扫描过程
- HandlerMapping选择策略
- HandlerAdapter选择策略
- ViewResolver选择策略
# 二、Spring IOC/DI
- Bean生命周期 
- IOC和DI流程
  - 问题
    1. @ComponentScan注解实现原理  
    2. @Configuration和@Bean与application.xml配置
- 如何控制单例和多例
- 如何控制延迟加载
- 事件监听机制
# 三、Spring AOP
- cglib和jdk动态代理实现AOP的具体流程
- 代理方式选择
  - 问题：
    1. 哪种情况下选择哪种代理模式，Spring是怎么控制选择哪种代理模式的？
- 拦截器实现原理
- 切面事务实现原理
- @Transactional事务实现原理
  - 问题：
    1. 为什么只回滚异常异常
    2. 手动异常回滚是怎么做的
# 四、Spring Boot
- Bean组件扫描和自动配置策略
  - 问题
    1. @SpringBootApplication 注解原理
    2. @Conditional注解实现原理
    3. @EnableAutoConfiguration注解实现原理
- 内置Tomcat原理
  - 问题
    1. 为什么不需要配置web.xml
    2. 为什么不需要部署外部tomcat
- 起步依赖原理
- 启动流程



