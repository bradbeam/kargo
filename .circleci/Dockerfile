FROM alpine:3.6

COPY requirements.txt /requirements.txt

RUN apk add --no-cache bash \
                       gcc \
                       git \
                       libffi-dev \
                       make \
                       musl-dev \
                       openssl-dev \
                       py-cffi \
                       py-pip \
                       python-dev && \
    pip install -r /requirements.txt

ENTRYPOINT [ "ansible-playbook" ]
