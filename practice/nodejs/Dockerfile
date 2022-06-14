# 1. node 설치
FROM node:12-alpine
# FROM    ubuntu:20.04
# RUN     apt-get update
# RUN     DEBIAN_FRONTEND=noninteractive apt-get install -y nodejs

# 2. 소스 복사
COPY   server.js /app/

# 3. WEB 서버 실행 (Listen 포트 정의)
EXPOSE 8080
CMD    ["node", "/app/server.js"]
