FROM fedora

MAINTAINER Giuseppe Scrivano <gscrivan@redhat.com>

RUN dnf install -y flannel

LABEL RUN /usr/bin/docker run --net=host --ipc=host -d \$OPT1 --name \$NAME \$IMAGE \$OPT2 \$OPT3

CMD ["/usr/bin/flanneld", "-etcd-endpoints=http://127.0.0.1:2379"]
