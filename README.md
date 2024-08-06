# Covid-19 Cases on Worldmap (Batch Processing)
 
-> It would be kind of batch pipeline where you will read 1 year of covid-19 data 
   (Confirmed, Recovered, Deaths) for each country date wise, process the data and 
   aggregate it, store processed data in mysql/nosql database, visualize data on worldmap. 
   So what steps & technology you can follow, let me explain about it..

- Download file from git repo and save it in your local

- Setup hadoop in local, here you need to focus on only two main components of hadoop (hdfs & yarn)

- since hdfs is dist file system so now copy that file from local to hdfs

- setup spark in your local

- write a spark application which reads file from hdfs and creates a dataframe

- aggregate data in spark application

- write aggregated data in output table using transactional database like mysql/postgres or any nosql
 database like cassandra/HBase .. as a beginner level i would say go with mysql because you can easily
 setup it in your local and it would be easy to use as well for dummy projects
 
- you can use any dashboarding tool like tableau, powerbi, grafana, kibana. but for this usecase 
  i would recommend to go with grafana because it is open source and good thing
  
- setup grafana in local

-install plugin for worldmap

-connect grafana to mysql


