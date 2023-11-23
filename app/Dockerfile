
FROM openjdk:11 as BUILD_IMAGE
RUN apt update && apt install git maven -y
RUN git clone https://bitbucket.org/dptrealtime/java-login-app.git
RUN cd java-login-app && mvn install




FROM tomcat:9-jre11
RUN rm -rf /usr/local/tomcat/webapps/*
COPY --from=BUILD_IMAGE java-login-app/target/dptweb-1.0.war /usr/local/tomcat/webapps/ROOT.war
