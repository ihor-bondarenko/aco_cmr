# aco_cmr
# aco_cmr
# aco_cmr
#start docker with mysql

docker run -it --link aco-mysql:mysql -p 7010:80 image:tag

#start mysql docker 

docker run --name aco-mysql -v /var/www/localhost/htdocs/mysqldb:/var/lib/mysql -e MYSQL_ROOT_PASSWORD="aco" -d image:latest


#attach to docker shell 

docker exec -it some-mysql bash
