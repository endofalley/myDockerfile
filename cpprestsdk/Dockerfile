FROM ubuntu:16.06
MAINTAINER liyl<liyl@sysware.com.cn>
RUN apt-get update && apt-get -y --no-install-recommends install \
                                libmodbus5 liblog4cxx10v5 \
                                libboost-regex1.58.0 libboost-system1.58.0 \
                                libboost-program-options1.58.0 libboost-thread1.58.0 \
                                libboost-filesystem1.58.0 libpthread-workqueue0 \
                                libssl1.0.0 libcpprest2.8 autotools-dev build-essential
RUN apt-get autoremove -y && \
    apt-get clean && rm -r /var/lib/apt/lists/*