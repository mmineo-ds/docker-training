Web container
docker build -t web-image:1.0 .
docker run --name web --link mysql:mysql -d -p 80:80 -v /home/Docker-training/docker-final-project-master/worldapi:/opt/www/worldapi wen-image:1.0

MySQL container
docker run --name mysql -e MYSQL_ROOT_PASSWORD=123456 -e MYSQL_DATABASE=dbdemo -e MYSQL_USER=devspark -e MYSQL_PASSWORD: dev123 -d mysql:5.6
