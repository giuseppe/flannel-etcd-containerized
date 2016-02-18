FROM fedora

MAINTAINER Giuseppe Scrivano <gscrivan@redhat.com>

RUN dnf install -y flannel && dnf clean all

ADD service.template /exports/service.template
ADD config.json /exports/config.json
