FROM registry.cn-hangzhou.aliyuncs.com/gospel/vd:app

MAINTAINER sharkseven 'shark@dodora.cn'

RUN rm -rf /root/temp
RUN git clone https://github.com/Gospely/vdpc-seed /root/temp
RUN bash -c ". /root/.nvm/nvm.sh && nvm use v6.9.1  && cd /root/temp && npm install"

EXPOSE 8060 80

ENTRYPOINT service ssh start && /config/main && /bin/bash
