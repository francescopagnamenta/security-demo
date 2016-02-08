
## Intro

Simple spring security web application (based on the official spring security samples). The demo application can be build and deployed on a Apache Tomcat server run with Docker.

## Create the Tomcat Docker container

cd docker

sudo docker build -t="keko/spring-security" .

sudo docker run -it --rm -p 8888:8080 keko/spring-security

## Build the project

mvn clean install

## Deploy the war locally

mvn tomcat7:deploy

## Test it

localhost:8888/sample/

