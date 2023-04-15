# Dockerfile

**Membuat Aplikasi PHP Menjadi Image Docker**

```
$ docker build -t sacode-php:1.1 .
```

**Membuat & Menjalankan Aplikasi PHP menggunakan Image yang dibuat sebelumnya**

```
$ docker run -it --rm --name my-sacode-app -p 8080:80 sacode-php:1.1
```

**Access Database Interactive Terminal**

```
$ docker exec -it nama_container_mysql mysql -u root -p
```

**Buka Aplikasi PHP di Browser:** 

- ```localhost:8080```

**Buka PHPMyAdmin di Browser:** 

- ```localhost:8081```


**Upload Images ke Docker Registry**

```
$ docker tag sacode-php:1.1 YOUR_DOCKERHUB_USER/sacode-php
$ docker login
$ docker push YOUR_DOCKERHUB_USER/sacode-php
```
