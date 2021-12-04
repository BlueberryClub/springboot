# spring的学习
  ## 第一天 spring框架的概述以及spring中基于XML的IOC配置
  ### 1. spring的概述：
  #### 1.1 spring是个什么：
  
    是为了解决企业级应用开发的复杂性而创建的框架（简化开发）
  
  #### 1.2 spring的两大核心：
  
    IOC（控制反转）：
    
    AOP（面向切面编程）：
    
  #### 1.3 spring的发展历程和优势：
  
    方便解耦，简化开发：
    
    AOP编程的支持：
    
    声明式事务的支持：
     
    方便程序的测试：
    
    方便集成各种优秀框架：
    
    降低javaEE API的使用难度：
    
    java源码是经典学习范例：
  
  #### 1.4 spring体系结构
  
  ### 2. 程序的耦合及解耦
  #### 2.1 曾经案例中的问题
  
    // 1. 注册驱动
    DriverManager.registerDriver(new com.mysql.jdbc.Driver());
    // 2. 获取连接
    Connection conn = DriverManager.getConnection("jdbc:mysql://localhost:3306/ssm","root","root");
    // 3. 获取操作数据库的预处理对象
    PreparedStatement pstm = conn.prepareStatement("select * from user");
    // 4. 执行SQL，得到结果集
    ResultSet resultSet = pstm.executeQuery();
    // 5. 遍历结果集
    while (resultSet.next()){
        System.out.println(resultSet.getString("userName"));
    }
    // 6. 释放资源
    resultSet.close();
    pstm.close();
    conn.close();
    
    // 具体的耦合与内聚的介绍：https://www.cnblogs.com/jiang-bei/articles/15522241.html
  
  #### 2.2 工厂模式解耦
  ### 3. IOC的概念和spring中的IOC
  #### 3.1spring中基于XML的IOC环境搭建
  ### 4. 依赖注入（Dependency Injection） 
       

  ## 第二天 spring中基于注解的IOC和ioc的案例


  ## 第三天 spring中的aop和基于xml以及注解的aop


  ## 第四天 spring的jdbcTemlate以及Spring的事务控制





