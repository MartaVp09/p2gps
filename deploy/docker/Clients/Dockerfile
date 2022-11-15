FROM tomcat:7-jre8

MAINTAINER marta.valiente1@alu.uclm.es

COPY drop/* /usr/local/tomcat/webapps/

EXPOSE 8082

ENTRYPOINT P=8082 ;sed "s/8080/$P/g" < conf/server.xml > /tmp/srv.xml && catalina.sh run -config /tmp/srv.xml
