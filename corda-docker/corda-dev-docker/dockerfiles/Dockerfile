# corda-testnet docker image

# Ubuntu 16.04 LTS (xenial)
FROM blockchain101/ubuntu16.04-dev:jdk8-maven3-gradle2-git
MAINTAINER Peng Zhuang <zhuangpeng0514@sina.com>

# copy the corda-testnet resource files into the image
ADD corda-settings.tar /corda-testnet

# change to work directory
WORKDIR /corda-testnet

# get the specified release of corda and cordapp-template
RUN git clone -b release-M6 https://github.com/corda/cordapp-template.git
RUN git clone -b release-M6 https://github.com/corda/corda.git

# build cordapp-template
ADD cordapp-template-resources.tar /corda-testnet
ADD cordapp-gradle-local-repository.tar /corda-testnet
RUN bash ./cordapp-template-deployNodes.sh

# change to work directory
ADD cordapp-template-startNode.tar /corda-testnet














