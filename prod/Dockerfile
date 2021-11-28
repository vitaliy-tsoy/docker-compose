FROM alpine
WORKDIR /tmp
RUN apk add --no-cache openjdk8-jre && rm -rf /var/cache/apk/* && rm -rf /etc/apk/* && wget https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.73/bin/apache-tomcat-8.5.73.tar.gz && mkdir /opt/tomcat && tar xvzf apache-tomcat-8.5.73.tar.gz -C /opt/tomcat --strip-components=1 && rm -rf /tmp/* && rm -rf /var/tmp/* && rm -rf /opt/tomcat/webapps/*
EXPOSE 8080
CMD /opt/tomcat/bin/catalina.sh run
