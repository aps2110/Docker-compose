FROM maven:3.8.6-openjdk-11
WORKDIR /app
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
RUN mvn -f /app/boxfuse-sample-java-war-hello/pom.xml package
VOLUME /mydata
RUN cp /app/boxfuse-sample-java-war-hello/target/hello-1.0.war /mydata
