FROM centos

RUN yum install -y curl bash epel-release gettext-devel && yum install -y jq

COPY check /opt/resource/check
COPY in    /opt/resource/in
COPY out   /opt/resource/out

RUN chmod +x /opt/resource/out /opt/resource/in /opt/resource/check

ADD test/ /opt/resource-tests/
RUN /opt/resource-tests/all.sh \
 && rm -rf /tmp/*
