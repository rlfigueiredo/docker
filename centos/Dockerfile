FROM centos
ENV scripts /scripts
#WORKDIR ${scripts}
#ADD https://github.com/rlfigueiredo/docker $scripts
ADD . $scripts/test
#COPY mounting-pi-nfs.sh $scripts
RUN yum install wget -y && \
yum install openssl -y && \
yum install tcpdump -y && \
yum install bind-utils -y \
yum install git -y \
yum install nmap -y \
yum install file -y
