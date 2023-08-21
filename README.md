# tomcat_docker

This Dockerfile is a Sample Dockerfile to create Tomcat of any version . 

Instructions to build 
===================== 
clone repo
>git clone <>
>cd tomcat_docker
>docker image build -t akreddy403/tomcat_docker:v1 .
>docker container run -itd --name=tomcatimage -p 90:8080 -p akreddy403/tomcat_docker:v1

Note: we can pass any version of tomcat we wish 

>docker image build -t akreddy403/tomcat_docker:v2 --build-arg tomcat_version=8.5.8 .
>
>docker container run -itd --name=tomcatimage -p 90:8080 -p akreddy403/tomcat_docker:v1
>
>access application check tomcat version
