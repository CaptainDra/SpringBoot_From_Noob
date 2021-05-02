# 关于Springboot框架的一些基础逻辑与初始创建

## Springboot框架结构分层
1. DAO层： 就是其他结构的mapper层，包括各种xxxmapper.java（数据库访问接口类）以及xxxmapper.xml（数据库连接实现）
2. Bean层：对应MVC框架model层，存放实体，数据库映射实体存放处
3. Service层：服务层，放各种业务，包含xxxservice.java(业务接口类)以及xxxserviceImpl(业务实现拓展类)，可以将两类分开存放，也可以将implement存在service包下
4. Web层：对应MVC的controller层，实现与前端的交互，view层一般单独存在外面

## 从创建开始
所使用IDEA版本为2021.2.4版本，不同版本可能会有出入    
1. File -> New -> Project 新建一个项目
2. 使用Spring Initializr, 我使用了自己一直用的JDK1.8
3. 改各种名称，主要后续用得上的是组名(Group)，和项目名称(Artifact)，以及将Java Version改为对应的8版本
4. 勾选Dependency，前期用得上的依赖包含：Web下的Spring Web，Template Engines下的Thymeleaf，SQL下的MySQL Driver，JDBC API，MyBatis Framework
5. 创建完毕，等就好了

### 创建完后需要检查的
1. 左侧的Maven，点击小扳手检查各种路径，然后Reload一下

