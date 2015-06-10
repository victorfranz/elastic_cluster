# elastic_cluster
Simple local elastic cluster for tests using vagrant + ansible + docker

It creates a virtual machine using vagrant on VirtualBox with 3 Docker containers with an elastic node each.

It uses angstwad/docker.ubuntu as a submodule dependence, so use clone with submodules: git clone --recursive https://github.com/victorfranz/elastic_cluster.git

To run, just: vagrant up
___
To see your cluster:

http://localhost:9201/_plugin/kopf/

http://localhost:9201/_plugin/HQ/

