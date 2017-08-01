# aco_cmr
# aco_cmr
# aco_cmr
#start docker with mysql
docker run -it --link aco-mysql:mysql -p 7010:80 obsd/aco-commander:0.1

#start mysql docker 
docker run --name aco-mysql -v /var/www/localhost/htdocs/mysqldb:/var/lib/mysql -e MYSQL_ROOT_PASSWORD="aco" -d obsd/aco_mysql:latest
