# tomcat_docker

This Dockerfile is a Sample Dockerfile to create Tomcat of any version . 

Instructions to build 
===================== 
clone repo
git clone <>
cd tomcat_docker
docker image build -t akreddy403/tomcat_docker:v1 .
docker container run -itd --name=tomcatimage -p 90:8080 -p akreddy403/tomcat_docker:v1

Note: we can pass any version of tomcat we wish 

docker image build -t akreddy403/tomcat_docker:v2 --build-arg tomcat_version=8.5.8 .

docker container run -itd --name=tomcatimage -p 90:8080 -p akreddy403/tomcat_docker:v1

access application check tomcat version


Note: lets make use of alpine image which consumes less space 

 docker image build -t tomcat_alpine2 -f Dockerfile_alpine .
 docker images
 docker container run -d --name=tomcat_container -p 9090:8080 tomcat_alpine2





