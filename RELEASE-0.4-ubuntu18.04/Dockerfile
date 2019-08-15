FROM ubuntu:18.04

RUN apt-get update

# https://github.com/tensorflow/swift/blob/master/Installation.md
RUN apt-get -y install clang libpython-dev libblocksruntime-dev

# Other stuff needed
RUN apt-get -y install libpython3.6 libxml2

COPY swift-tensorflow-RELEASE-0.4-ubuntu18.04.tar.gz .
RUN tar xzf swift-tensorflow-RELEASE-0.4-ubuntu18.04.tar.gz

RUN export PATH=$(pwd)/usr/bin:"${PATH}"

RUN swift --version
