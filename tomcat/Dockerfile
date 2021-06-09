FROM tomcat:9.0

# need the server.xml here
COPY ./server.xml /usr/local/tomcat/conf
COPY ./tomcat-users.xml /usr/local/tomcat/conf

# Enable Manager Application
RUN cp -R /usr/local/tomcat/webapps.dist/manager /usr/local/tomcat/webapps/
COPY ./context.xml-manager /usr/local/tomcat/webapps/manager/META-INF/context.xml

# deploy war here?
COPY ./sample.war /usr/local/tomcat/webapps/sample.war

# expose ajp13 port
EXPOSE 8009 8080