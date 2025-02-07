FROM postgres:14.7

ENV TZ Asia/Shanghai

RUN apt-get update && apt-get -y install pgagent=4.2.3-1 && \
    echo ${TZ} | tee /etc/timezone && \
    dpkg-reconfigure --frontend noninteractive tzdata