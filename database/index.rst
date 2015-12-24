.. _database-overview:

数据库
==========
\ **关系数据库**\ ：Mysql、Oracle、SQLite

\ **KV数据库**\ ：Memcached、Redis、Raik（Amazon）

\ **硬盘KV数据库**\ ：SSDB（LevelDb）

* LevelDB是单机存储引擎

\ **列形数据库**\ ：HBase、BigTable、Cassandra、Hypertable

* Cassandra是P2P的（无中心管理节点）

\ **文档数据库**\ ：MongoDB、CouchDB

\ **图数据库**\ ：Neo4j

	图数据库支持ACID规则以及自动索引


.. toctree::
   :maxdepth: 1
   :numbered: 2
    
   storeEngine
   tuning
   mysql
