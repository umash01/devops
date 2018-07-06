FROM centos

RUN yum install java-1.8.0-openjdk-devel.x86_64 -y

ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk

RUN yum install wget -y

RUN wget http://www-us.apache.org/dist/tomcat/tomcat-9/v9.0.10/bin/apache-tomcat-9.0.10.zip -O /tmp/tomcat.zip

RUN yum install unzip -y

RUN unzip /tmp/tomcat.zip -d /opt

RUN chmod -R 755 /opt/apache-tomcat-9.0.10/bin

CMD bash -C /opt/apache-tomcat-9.0.10/bin/startup.sh; sleep infinity
