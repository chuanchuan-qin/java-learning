# Java工程师从零基础到就业

---

### 阶段一：Java 核心基础（约 5 周）
> **目标**：扎实掌握 Java 语法与面向对象思想，能编写控制台程序。

- **[环境配置](javaSE/day01-environment/1-java环境配置.md)**：安装 JDK 17、IDEA，配置环境变量
- **基础语法**：[变量与数据类型](javaSE/day02-variable/2-变量与数据类型.md)、运算符、流程控制、数组
- **面向对象**：类与对象、封装、继承、多态、抽象类、接口、内部类、枚举
- **核心类库**：String、包装类、日期时间（java.time）、异常处理、泛型、集合框架（List/Set/Map 及其实现类）、Collections 工具类
- **进阶特性**：Lambda 表达式、Stream API、Optional（Java 8+ 企业常用）
- **IO 与多线程基础**：File、字节/字符流、缓冲流；线程创建、同步、线程池、并发工具类（JUC）入门
- **练习**：完成一个**学生信息管理系统**，控制台交互，用集合或文件存储数据。

---

### 阶段二：数据库与 JDBC（约 3 周）
> **目标**：熟练写 SQL，能用 Java 操作数据库。

- **MySQL**：安装、数据类型、DDL/DML、单表/多表查询（JOIN）、子查询、聚合函数、事务、索引入门（Explain 分析）
- **JDBC**：驱动注册、Connection、PreparedStatement、ResultSet、封装工具类
- **连接池**：Druid 或 HikariCP 的基本使用
- **练习**：用 Java 控制台程序对数据库进行增删改查（如商品管理）。

---

### 阶段三：Web 基础与前端入门（约 3 周）
> **目标**：理解 B/S 架构，能跑通前后端交互流程。

- **前端基础**：HTML、CSS 基础、JavaScript、Ajax、axios，能看懂 Vue 脚手架项目结构即可
- **HTTP 协议**：请求/响应结构、状态码、GET/POST 区别、Cookie/Session 原理
- **Java Web**：Tomcat 使用、Servlet 生命周期、Request/Response、Filter、Listener、MVC 思想（JSP 了解即可）
- **工具链**：Maven 依赖管理、Git 版本控制、Postman 接口测试
- **练习**：不依赖框架，手写一个基于 Servlet 的登录注册小 Demo。

---

### 阶段四：主流框架与 Spring Boot（约 7 周）
> **目标**：能独立开发基于 Spring Boot 的单体 RESTful API 项目。

- **Spring**：IoC/DI（注解与 JavaConfig）、Bean 生命周期、AOP、声明式事务
- **Spring MVC**：RESTful 设计、请求参数绑定、统一异常处理、拦截器
- **MyBatis / MyBatis-Plus**：映射配置、动态 SQL、分页插件、代码生成器
- **Spring Boot**：自动配置原理（理解即可）、yaml 配置、多环境、starter 整合 MyBatis/Redis 等
- **项目一：企业级后台管理系统或博客系统**  
  技术栈：Spring Boot + MyBatis-Plus + MySQL + JWT + Swagger/Knife4j  
  功能：注册登录、文章/商品 CRUD、分类管理、权限控制（Spring Security 或 Shiro 了解即可）、统一返回格式、日志
- **测试与部署**：JUnit5 单元测试，打包成 Jar，在 Linux 服务器上部署（可用虚拟机）

---

### 阶段五：中间件与微服务（约 7 周）
> **目标**：掌握高可用、高并发核心组件，具备开发微服务架构项目的能力。

- **Redis**：五大数据类型、持久化（RDB/AOF）、缓存穿透/击穿/雪崩解决方案、分布式锁（Redisson）、Spring Boot 整合 Redis 实现缓存
- **消息队列**：RabbitMQ 或 RocketMQ，掌握消息模型、可靠性投递、死信队列、削峰解耦，Spring Boot 整合实现异步处理
- **Linux 与 Docker**：Linux 常用命令、日志查看、Docker 镜像/容器、Dockerfile、Docker Compose 编排，将项目容器化部署
- **微服务入门**（Spring Cloud Alibaba）：
    - Nacos 注册中心/配置中心
    - OpenFeign 远程调用
    - Gateway 网关（路由、鉴权）
    - Sentinel 流量控制与降级
    - 了解分布式事务概念（Seata）
- **并发与 JVM 深入**（为面试打下基础）：
    - 线程池原理与参数、volatile、CAS、synchronized、Lock、ConcurrentHashMap
    - JVM 内存结构、类加载、垃圾回收算法、常用调优参数、OOM 排查思路
- **项目二：高并发秒杀系统或外卖点餐系统**  
  技术栈：Spring Boot + Spring Cloud Alibaba + MyBatis-Plus + Redis + RabbitMQ + Docker + Nginx  
  亮点：服务拆分、缓存预热、MQ 异步下单减库存、分布式锁防超卖、限流保护、容器化部署。

---

### 阶段六：就业冲刺与面试准备（约 4 周）
> **目标**：完善简历与项目，通过高频面试考察。5t

- **项目包装**：用 STAR 原则描述项目，突出技术难点、QPS 优化、业务模型
- **算法与数据结构**：每日 2~3 道 LeetCode（简单/中等），重点：数组、链表、树、栈/队列、二分、动态规划入门
- **高频面试题**：
    - Java 基础：HashMap 原理、ArrayList 与 LinkedList、String 不可变、反射、动态代理
    - 并发：线程池、锁升级、AQS 原理、ThreadLocal
    - JVM：内存模型、垃圾回收器、调优经验
    - 框架：Spring IOC/AOP 原理、Bean 生命周期、循环依赖解决、Spring Boot 自动配置、MyBatis 执行流程
    - 数据库：索引结构（B+Tree）、SQL 优化、分库分表概念
    - 分布式：CAP 理论、Base 理论、分布式锁、幂等性设计、缓存与数据库一致性
- **设计模式**：单例、工厂、代理、策略、模板方法，能手写单例
- **简历与投递**：突出两个项目经历，技术栈与 JD 匹配；模拟面试，录音复盘

---

### 一些重要的提醒
- **动手优先**：每个阶段至少要完成对应的练习或项目，不能只看视频。
- **笔记与博客**：用 Markdown 记录核心知识点，既复习也作为面试素材。
- **不要贪多**：初级开发岗位不需要精通所有微服务组件，但 Spring Boot、MySQL、Redis、RabbitMQ 的主流用法必须能清晰说清并写出来。
- **持续迭代**：项目可以不断加功能，比如引入 Elasticsearch 实现搜索、用 Canal 同步数据，让简历更有竞争力。

按照这条路线坚持学完，你就具备了大多数互联网公司对 **Java 初级/中级后端开发** 的硬性要求。找工作除了技术，学历、沟通表达和面试节奏也很重要，但扎实的项目经历始终是敲门砖。祝你顺利转行上岸！