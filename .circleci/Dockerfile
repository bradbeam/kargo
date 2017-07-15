FROM alpine:3.6

COPY requirements.txt /requirements.txt

RUN apk add --no-cache bash \
                       curl \
                       gcc \
                       git \
                       jq \
                       libffi-dev \
                       make \
                       musl-dev \
                       openssl-dev \
                       py-cffi \
                       py-pip \
                       python-dev \
                       openssh-client \
                       tar && \
    pip install -r /requirements.txt

ENTRYPOINT [ "ansible-playbook" ]
