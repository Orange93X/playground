FROM tomcat:9.0.79-jdk17-corretto

RUN chmod -R 777 /usr/local/tomcat
ENV export CATALINA_OPTS="-DJENKINS_HOME=/usr/local/tomcat -Xmx512m"

RUN yum -y install wget

RUN wget -P /usr/local/tomcat/webapps/ https://get.jenkins.io/war/2.420/jenkins.war
RUN wget -P /usr/local/tomcat/webapps/ https://tomcat.apache.org/tomcat-7.0-doc/appdev/sample/sample.war
