FROM fedora
ENV scripts /scripts
#WORKDIR ${scripts}
#ADD https://github.com/rlfigueiredo/docker $scripts
#ADD . $scripts/test
#COPY mounting-pi-nfs.sh $scripts
RUN yum install wget openssl tcpdump bind-utils git nmap file net-tools file -y \
&& wget https://github.com/cloudfoundry/bosh-cli/releases/download/v5.3.1/bosh-cli-5.3.1-linux-amd64 \
&& mv bosh-cli-5.3.1-linux-amd64 /usr/local/bin/bosh \
&& chmod 755 /usr/local/bin/bosh \
&& git clone https://github.com/rlfigueiredo/docker.git $scripts/docker
#RUN yum install wget -y \
#&& yum install openssl -y \
#&& yum install tcpdump -y \
#&& yum install bind-utils -y \
#&& yum install git -y \
#&& yum install nmap -y \
#&& yum install file -y \
#&& yum install net-tools -y \
#&& yum install file -y
