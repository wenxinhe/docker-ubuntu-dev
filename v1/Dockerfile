FROM wenxinhe/ubuntu:14.04

# jdk
COPY jdk1.8.0_40 /opt/jdk1.8.0_40/
RUN echo "export JAVA_HOME=/opt/jdk1.8.0_40" >> /etc/profile
RUN echo "export PATH=\$JAVA_HOME/bin:\$PATH" >> /etc/profile

#RUN apt-get update && apt-get install -y openjdk-7-jdk
#COPY java.sh /etc/profile.d/

#maven
COPY apache-maven-3.2.3 /opt/apache-maven-3.2.3
RUN echo "export M3_HOME=/opt/apache-maven-3.2.3" >> /etc/profile
RUN echo "export PATH=\$M3_HOME/bin:\$PATH" >> /etc/profile 

RUN chmod +x /etc/profile.d/*.sh


