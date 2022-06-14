# 1. node 설치
# 누군가 우분투에 node js를 설치해놓은 이미지, 밑에 3개가 다 포함됨
#FROM node:12
# 용량 줄인 버전(사용하지않는건 포함 안됨)
FROM node:12-alpine
#FROM    ubuntu:20.04
#RUN     apt-get update
#RUN     DEBIAN_FRONTEND=noninteractive apt-get install -y nodejs npm

# 2. 소스 복사
COPY    . /usr/src/app

# 3. Nodejs 패키지 설치
WORKDIR /usr/src/app
RUN     npm install

# 4. WEB 서버 실행 (Listen 포트 정의)
EXPOSE 3000
CMD    node app.js