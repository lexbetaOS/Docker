# Docker

### 1. Commands to create image for Dockerfile which contain html files for personal blog.

```bash
docker build --tag centos_apache:v1 .
docker images
docker run -d -p 9090:80 --name centos-yescmd centos_apache:v1
docker ps
```

![image](https://user-images.githubusercontent.com/9786713/178168558-065c9b65-c88f-44ac-98da-072c8716ddb3.png)

### 2. Commands to create image for Dockerfile2 which contain html files.


```bash
docker rm -f centos-yescmd
docker build -t nginx_custom:v1 -f Dockerfile2 .
docker images
docker run -d -p 9090:80 --name nginx nginx_custom:v1
docker ps
```
![image](https://user-images.githubusercontent.com/9786713/178357367-5d2fa570-4321-4ede-9012-6f7c79ff812f.png)
