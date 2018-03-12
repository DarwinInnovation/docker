FROM gcc:7

RUN apt-get update && apt-get install -y --no-install-recommends \
    wget git \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
RUN wget https://cmake.org/files/v3.10/cmake-3.10.2.tar.gz && tar -xzf cmake-3.10.2.tar.gz && rm -f cmake-3.10.2.tar.gz && cd cmake-3.10.2 && ./bootstrap --prefix=/usr && make && make install && cd .. && rm -rf cmake-3.10.2

