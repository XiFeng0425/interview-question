### Dapper是一款轻量级的ORM工具（Github）。
如果你在小的项目中，使用EntityFramework、NHibernate来处理
大数据访问及关系映射，未免有点杀鸡用牛刀了。你又觉得ORM省时省力
这里Dapper将是不二选择。
### Dapper的优点：
1. 轻量。只有一个文件（SqlMapper.cs) ，编译完成之后只有120k（好像是变胖了）。
2. 速度快。Dapper的速度接近与IDataReader，取列表的数据超过了DataTable.
3. 支持多种数据库。Dapper可以在所有ADO.NET providers 下工作，
 包括sqllite,sqlce,firebird,oracle,mysql,postgresql ,sqlserver
4. 可以映射一对一，一对多，多对多等多种关系。
5. 性能高。通过Emit反射DataReader的序列队列，来快速的得到和产生对象，
性能不错。
6. 支持FrameWork2.0 3.0 3.5 4.0 4.5
  
  