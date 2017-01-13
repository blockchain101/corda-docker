# corda-testnet-docker
docker files create blockchain101/corda-testnet based on blockchain101/ubuntu16.04-dev:jdk8-maven3-gradle2-git in docker hub
docker compose file to run docker containers using above blockchain101/corda-testnet image
4 corda nodes containers: corda-controller, corda-nodea, corda-nodeb, corda-nodec
NOTE:
Before startup in dockercompose file, be sure using default docker bridge network: 172.17.0.0/24, otherwise please change hosts file
configered ip address for each node container
172.17.0.2      corda-controller
172.17.0.5      corda-nodea
172.17.0.4      corda-nodeb
172.17.0.3      corda-nodec
create a ~/cordadata as host owned directory and put hosts file in it.

# corda-dev-docker
docker files create blockchain101/corda-dev based on blockchain101/ubuntu16.04-dev:jdk8-maven3-gradle2-git in docker hub
docker compose file to run docker containers using above blockchain101/corda-dev image
4 corda nodes containers: corda-controller, corda-nodea, corda-nodeb, corda-nodec
NOTE:
Before startup in dockercompose file, be sure using default docker bridge network: 172.17.0.0/24, otherwise please change hosts file
configered ip address for each node container
172.17.0.2      corda-controller
172.17.0.5      corda-nodea
172.17.0.4      corda-nodeb
172.17.0.3      corda-nodec
create a ~/cordadata as host owned directory and put hosts file in it.

# ubun-dev-docker
docker files create blockchain101/ubuntu16.04-dev based on ubuntu:16.04 in docker hub
this dev image appended with jdk1.8 maven3 gradle2 and git installed and served as base image of blockchain101/corda-testnet and blockchain101/corda-dev

