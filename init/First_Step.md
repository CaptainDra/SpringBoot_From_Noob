# 关于Springboot框架的一些基础逻辑与初始创建

## Springboot框架结构分层
1. DAO层： 就是其他结构的mapper层，包括各种xxxmapper.java（数据库访问接口类）以及xxxmapper.xml（数据库连接实现）
2. Bean层：对应MVC框架model层，存放实体，数据库映射实体存放处
3. Service层：服务层，放各种业务，包含xxxservice.java(业务接口类)以及xxxserviceImpl(业务实现拓展类)，可以将两类分开存放，也可以将implement存在service包下
4. Web层：对应MVC的controller层，实现与前端的交互，view层一般单独存在外面


