FROM alpine:edge

RUN echo -e "https://mirror.tuna.tsinghua.edu.cn/alpine/edge/main\nhttps://mirror.tuna.tsinghua.edu.cn/alpine/edge/community\n" > /etc/apk/repositories

RUN apk update

RUN apk add --no-cache nginx uwsgi uwsgi-python3 python3 py3-pip && ln -fs /usr/bin/python3 /usr/local/bin/python && pip install pipenv
