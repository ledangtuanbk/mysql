# mysql 
custom mysql
# run 
docker run --name CONTAINER_NAME --restart=always -v VOLUME_NAME:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=1 -d -p 3306:3306 ledangtuanbk/mysql:5.7
# backup
docker exec -t mysql mysqldump -u root -p PASSWORD DATABASE_NAME > /mnt/backup_`date +%d-%m-%Y"_"%H_%M_%S`.sql
