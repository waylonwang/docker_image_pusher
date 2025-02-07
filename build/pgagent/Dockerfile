FROM postgres:14.7

ENV TZ Asia/Shanghai

RUN apt-get update && apt-get -y install pgagent && \
    echo ${TZ} | tee /etc/timezone && \
    dpkg-reconfigure --frontend noninteractive tzdata