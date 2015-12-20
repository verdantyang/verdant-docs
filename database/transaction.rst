.. _transaction:

ACID表示原子性(atomicity)、一致性(consistency)、隔离性(isolation)、持久性(durability)

数据库事务级别 
================
**脏读（dirty read）:**

1. 事务T1更新了一行记录的内容，但是并没有提交所做的修改
2. 事务T2读取更新后的行，然后T1执行回滚操作，取消了刚才所做的修改
3. 现在T2所读取的行就无效了







