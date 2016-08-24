# dockertest
For testing integration with docker on digital ocean droplet
1. Created a javafile: HelloDockerWorld.java
2. Put it on the server with SFTP
3. Created a Dockerfile in same directory
FROM java:7
COPY HelloDockerWorld.java .
RUN javac HelloDockerWorld.java

CMD ["java", "HelloDockerWorld"]

4. 
