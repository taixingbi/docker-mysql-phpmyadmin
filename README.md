
docker pull mysql:5.7
docker pull phpmyadmin/phpmyadmin

docker run --name mysql1 -e MYSQL_ROOT_PASSWORD=admin  -d mysql:5.7
docker run --name phpmyadmin -d --link mysql1:db -p 8081:80 phpmyadmin/phpmyadmin

0.0.0.0:8081
user:root
password:admin
//youtube
https://www.youtube.com/watch?v=q8c4LiQj8EY


//----------------------- from docker-----------------
docker pull mysql/mysql-server

image: mysql/mysql-server
names: mysql1
password: admin

//mysql cmd

//access mysql1
docker exec -it mysql1 mysql -uroot -p

//access MySQL Server container
docker exec -it mysql1 bash

//exit from mysql
exit

