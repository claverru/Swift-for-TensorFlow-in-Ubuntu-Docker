FROM ubuntu:16.04

RUN apt-get update
RUN apt-get -y install curl
RUN apt-get install -y clang libicu-dev libpython-dev libncurses5-dev libxml2

# place file in the same location as Dockerfile
COPY swift-tensorflow-DEVELOPMENT-2018-08-15-a-ubuntu16.04.tar.gz .

RUN tar xzf swift-tensorflow-DEVELOPMENT-2018-08-15-a-ubuntu16.04.tar.gz

RUN export PATH=$(pwd)/usr/bin:"${PATH}"

CMD swift 
# -I/usr/lib/swift/clang/include
# option above was suposed to prevent some error in swift execution, doesn't seem to be needed 