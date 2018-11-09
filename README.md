# springboot-shardingjdbc  http://shardingsphere.io

说明：

    1. 克隆sharding-sphere 3.X 版本   git clone https://github.com/sharding-sphere/sharding-sphere
    2. 编译  mvn clean install -DskipTests
    3. 官网地址： http://shardingjdbc.io/index_zh.html
    4. 本项目单元测试 test



简介：

    1.框架
        spring boot
        io.shardingsphere.sharding-jdbc 3.0
        mybatis
        HikariCP
         
     
    2.数据库：
        在本地使用两个DB，分别为 test0,test1, sql脚本在项目中
        
        
    3.分库：
        使用 userId % 2 作为分库规则
        
        
    4.分表：
        使用 orderId % 2 作为分表规则
        
        
声明：

    1.sql支持与限制：
        支持聚合，分组，排序，分页，OR，关联查询等复杂查询语句
        支持DML，DDL，TCL以及数据库管理语句
        支持=，BETWEEN，IN的分片操作符
     
    
    2.读写分离
        一主多从的读写分离
        同一线程内的数据一致性
        支持分库分表与读写分离共同使用
        基于Hint的强制主库路由
    
    