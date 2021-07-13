from here:

https://spring.io/guides/gs/spring-boot-kubernetes/

run jenkins in container:
docker run -p 8080:8080 -p 50000:50000 -d -v /home/igor/Code/java-sandbox/containerized/jar-in-k8s/jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk11
with no mount volume:  
docker run -p 8080:8080 -p 50000:50000 -d jenkins/jenkins:lts-jdk11
