FROM centos:latest
USER root
RUN sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-Linux-*
RUN sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-Linux-*
RUN dnf update -y
# Mac
RUN dnf install -y java-11-openjdk-devel.aarch64
# Windows
#RUN dnf install -y java-11-openjdk-devel.x86_64

# # jar maven 프로젝트 실행
WORKDIR /root
CMD java -jar trade-0.0.1-SNAPSHOT.jar