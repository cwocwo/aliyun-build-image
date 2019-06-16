FROM registry.cn-beijing.aliyuncs.com/rdc-builds/base:1.0   
RUN sudo apt-get install -y software-properties-common && \
    sudo apt-get install -y python-software-properties && \
    sudo add-apt-repository ppa:openjdk-r/ppa && \
    sudo apt-get update && \
    sudo apt-get install -y openjdk-8-jdk
RUN cd /tmp && \
    wget https://services.gradle.org/distributions/gradle-5.2.1-bin.zip && \
    unzip gradle-5.2.1-bin.zip -d /srv/  && \
ENV PATH=${PATH}:/srv/gradle-5.2.1/bin
