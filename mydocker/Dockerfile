# To build use:
# docker build -t orian/cppenv:v1 .
FROM ubuntu:16.04
MAINTAINER Han Yu

LABEL description="A linux C++ build environment for pelaton"
ENV LD_LIBRARY_PATH=/libs
ENV CPLUS_INCLUDE_PATH=/libs/include

RUN mkdir /src
RUN mkdir /build
WORKDIR /build

COPY packages.sh /build
RUN bash /build/packages.sh

CMD ["/bin/bash"]
