# nginx-test2
```
1. Build
$ docker build --tag ohchang3/nginx-test2 .
Sending build context to Docker daemon  56.83kB
Step 1/4 : FROM ubuntu
 ---> 74435f89ab78
Step 2/4 : RUN apt update -y
 ---> Using cache
 ---> 8f1955656ea1
Step 3/4 : RUN apt install -y nginx
 ---> Using cache
 ---> 1ba4c57e40e7
Step 4/4 : CMD ["nginx", "-g", "daemon off;"]
 ---> Running in 11b9ec5e8176
Removing intermediate container 11b9ec5e8176
 ---> 57d9d527d487
Successfully built 57d9d527d487
Successfully tagged ohchang3/nginx-test2:latest
SECURITY WARNING: You are building a Docker image from Windows against a non-Windows Docker host. All files and directories added to build context will have '-rwxr-xr-x' permissions. It is recommended to double check and reset permissions for sensitive files and directories.

2. Run
$ winpty docker run -it --name n1 -p 8888:80 ohchang3/nginx-test2

![Screenshot](screenshot.png)




```
