## infs3208_individual_project

### Steps to Run
To start all containers  
`docker-compose up -d`  
  
Run the below commands to put the three source files into HDFS. Substitute <container_id> with
your namenode container ID. After that, you should see the three files from HDFS web interface at
http://external_IP/explorer.html  
`docker ps`  
`docker exec <container_id> hdfs dfs -put /home/nbs/links.csv /links.csv`  
`docker exec <container_id> hdfs dfs -put /home/nbs/movies.csv /movies.csv`  
`docker exec <container_id> hdfs dfs -put /home/nbs/ratings.csv /ratings.csv`  
`docker exec <container_id> hdfs dfs -put /home/nbs/tags.csv /tags.csv`  

