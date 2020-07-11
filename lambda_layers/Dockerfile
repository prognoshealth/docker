FROM lambci/lambda:build-python3.7
LABEL MAINTAINER="Cristian Capdevila ccapdevila@prognos.ai"

SHELL ["/bin/bash", "-c"]

RUN rpm --rebuilddb && \
    yum install -y yum-plugin-ovl && \
    yum clean all

RUN rpm --rebuilddb && \
    yum update -y && \
    yum install -y \
        atlas-devel \
        atlas-sse3-devel \
        blas-devel \
        gcc \
        gcc-c++ \
        lapack-devel \
        openssl-devel \
        findutils
