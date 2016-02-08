
Create the tomcat Docker container

cd docker

sudo docker build -t="keko/spring-security" .

sudo docker run -it --rm -p 8888:8080 keko/spring-security

Build the project

mvn clean install

Deploy the war locally

mvn tomcat7:deploy

Test it

localhost:8888/sample/

