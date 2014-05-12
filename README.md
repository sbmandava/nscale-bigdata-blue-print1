nscale-bigdata-blue-print1
==========================

nScale Application BigData Application Reference Architecture/Blueprint #1

Reference Multi-Tier Architecture to build a n-tier using Docker.

Components :

 Web-Tier
  Network Load Balancer (haproxy)
  WebServer (apache)

 Data-Tier
  Distributed Filesystem (Hadoop HDFS)
  Scalable SQL : Hive
  KeyValue Store : Hbase.
  In-Memory Store : Spark

 Search 
  Elastic Search

 Presentation 
  Kibana
