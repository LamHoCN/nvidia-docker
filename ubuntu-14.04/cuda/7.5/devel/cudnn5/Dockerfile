FROM cuda:7.5-devel
LABEL maintainer "NVIDIA CORPORATION <cudatools@nvidia.com>"

RUN echo "deb http://developer.download.nvidia.com/compute/machine-learning/repos/ubuntu1404/x86_64 /" > /etc/apt/sources.list.d/nvidia-ml.list

ENV CUDNN_VERSION 5
LABEL com.nvidia.cudnn.version="5"

RUN apt-get update && apt-get install -y --no-install-recommends \
            libcudnn5-dev=5.1.3-1+cuda7.5 && \
    rm -rf /var/lib/apt/lists/*
