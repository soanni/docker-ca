FROM openjdk:8-jdk-alpine
ENV MAVEN_VERSION=3.3.9
RUN cd /tmp && \
    wget -q "http://apache.ip-connect.vn.ua/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz" && \ 
    tar -xzf "apache-maven-$MAVEN_VERSION-bin.tar.gz" && \
    mv "/tmp/apache-maven-$MAVEN_VERSION" /usr/lib && \
    ln -s /usr/lib/apache-maven-3.3.9/bin/mvn /usr/bin/mvn && \
    rm "/tmp/apache-maven-$MAVEN_VERSION-bin.tar.gz"
COPY . /usr/src/journal
