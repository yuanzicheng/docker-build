FROM alpine:edge
# RUN echo -e "https://mirror.tuna.tsinghua.edu.cn/alpine/edge/main\nhttps://mirror.tuna.tsinghua.edu.cn/alpine/edge/community\n" > /etc/apk/repositories
RUN echo -e "https://mirrors.aliyun.com/alpine/edge/main\nhttps://mirrors.aliyun.com/alpine/edge/community\n" > /etc/apk/repositories
RUN apk update
RUN apk add --no-cache nginx uwsgi uwsgi-python3 python3 python3-dev py3-pip && ln -fs /usr/bin/python3 /usr/local/bin/python && pip install pipenv
ENV LANG=C.UTF-8

# FROM nginx-uwsgi-python3-dev:alpine-edge

