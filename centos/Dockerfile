FROM centos
ENV scripts /scripts
#WORKDIR ${scripts}
#ADD https://github.com/rlfigueiredo/docker $scripts
#ADD . $scripts/test
#COPY mounting-pi-nfs.sh $scripts
RUN yum install wget -y && \
yum install openssl -y && \
yum install tcpdump -y && \
yum install bind-utils -y \
yum install git -y \
yum install nmap -y \
<<<<<<< HEAD
yum install file -y \
yum install net-tools -y
=======
yum install file -y
RUN git clone https://github.com/rlfigueiredo/docker.git $scripts/docker
>>>>>>> c4bab93c98ebfbed426a04d6e4dca5d9543415ee
