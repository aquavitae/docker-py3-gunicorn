FROM centos:6

RUN yum -y update && yum clean all && yum -y install wget
RUN wget -O /etc/yum.repos.d/home:jsuarezr:LibrePlan.repo download.opensuse.org/repositories/home:/jsuarezr:/LibrePlan/CentOS_CentOS-6/home:jsuarezr:LibrePlan.repo
RUN yum -y install libreplan

EXPOSE 8080
