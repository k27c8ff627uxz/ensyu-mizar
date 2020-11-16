FROM node

RUN apt update
RUN npm install -g yo generator-code

WORKDIR /root/work
ADD mizar.tar /root/work

RUN yes '' | ./install.sh
ENV MIZFILES /usr/local/share/mizar

WORKDIR /
RUN rm -rf /root/work
