# docker
완벽한 IT 인프라 구축을 위한 Docker 2판

## Contents
- Docker setup

## Environment
> Client tool - Docker for Windows [Docker Engine 19.03.2] (https://hub.docker.com/editions/community/docker-ce-desktop-windows)<br />
OS - Windows 10 Pro

## Useful site
- Docker Toolbox (https://docs.docker.com/toolbox/)
- Nginx image (https://hub.docker.com/_/nginx)

## Docker Setup
> Hello World 출력<br /><br />
`$ docker container run ubuntu:latest /bin/echo 'Hello World!'`
<br />

> Docker Version 확인<br /><br />
`$ docker version`
<br />

> Docker 실행 환경 확인<br /><br />
`$ docker system info`
<br />

> Docker Disk 이용 상황 확인<br /><br />
`$ docker system df`<br />
`$ docker system df -v`
<br />

> Docker Nginx Image Download<br /><br />
`$ docker pull nginx`<br />
`$ docker image ls`
<br />

> Nginx 작동 (Docker image 'nginx'를 사용하여 'webserver'라는 이름의 Docker container run<br />
 (명령어 실행하면 container id 출력됨)<br /><br />
`$ docker container run --name webserver -d -p 80:80 nginx`<br />
localhost:80 치면 nginx 탑 화면 노출
<br />

> Docker로 기동시킨 Nginx 서버 상태 확인<br /><br />
`$ docker container ps`
<br />

> 'webserver' container 상세 확인<br /><br />
`$ docker container stats webserver`
<br />

> Container stop<br /><br />
`$ docker stop webserver`<br />
localhost:80 치면 error 화면 노출
<br />

> Container start<br /><br />
`$ docker start webserver`
<br />

