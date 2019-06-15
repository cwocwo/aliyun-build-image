FROM registry.cn-beijing.aliyuncs.com/rdc-builds/base:1.0   
RUN cd /tmp && \
    wget https://download.oracle.com/otn/java/jdk/8u211-b12/478a62b7d4e34b78b671c754eaaf38ab/jdk-8u211-linux-x64.tar.gz?AuthParam=1560593066_cb713881f55183f43bc66dad21d1b858 && \
    tar xf jdk-8u211-linux-x64.tar.gz -C /srv/java && \
    ln -s /srv/java/jdk* /srv/java/jdk 
ENV JAVA_HOME=/srv/java/jdk \
    PATH=${PATH}:/srv/java/jdk/bin:/srv/java
RUN apt-get install -y unzip    
RUN cd /tmp && \
    wget https://services.gradle.org/distributions/gradle-5.2.1-bin.zip && \
    unzip gradle-5.2.1-bin.zip -d /srv/  && \
ENV PATH=${PATH}:/srv/gradle-5.2.1/bin
