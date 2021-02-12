FROM centos:latest

RUN yum install python3 -y

RUN python3 -m pip install -U pip

RUN pip install ansible

RUN mkdir /etc/ansible/

RUN echo >> /root/ip.txt

RUN yum install wget -y

RUN wget https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm

RUN rpm -ivh epel-release-latest-8.noarch.rpm

RUN yum install sshpass -y

COPY ansible.cfg  /etc/ansible/
