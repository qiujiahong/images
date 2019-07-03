FROM centos:7.6.1810 


COPY  softwares/jdk-8u211-linux-x64.tar.gz  /

RUN  mkdir /apps && \
     tar -xzvf /jdk-8u211-linux-x64.tar.gz -C /apps/  && \
     cd /apps/ && \
     mv jdk1.8.0_211/ jdk8 && \
    #  echo "export JAVA_HOME=/apps/jdk8"  >> /etc/profile && \
    #  echo "export PATH=\$JAVA_HOME/bin:$PATH">> /etc/profile && \
    #  source /etc/profile  && \
     rm -rf /jdk-8u211-linux-x64.tar.gz 

ENV JAVA_HOME /apps/jdk8
ENV PATH $JAVA_HOME/bin:$PATH
     