Run Flannel and Etcd in a runc container on Fedora Atomic Host
======

It requires that the Fedora Atomic Host system has ```runc``` installed.

There are two different Ansible playbooks:

* playbook-docker.yml: It generates the runc rootfs for Flannel and
Etcd from a Docker container.

* playbook-rpm-ostree.yml: It uses rpm-ostree to create the
containers. One advantage is that files are hard linked, so the same
files, even if used by different containers, do not take additional disk space.

