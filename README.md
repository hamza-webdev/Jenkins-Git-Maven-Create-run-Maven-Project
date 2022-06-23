# Jenkins-Git-Maven-Create-run-Maven-Project
# Jenkins-Git-Maven-Create-run-Maven-Project
* mvn clean
* mvn clean test
* mvn clean package
* mvn clean package install
* mvn -Dmaven.test.skip=TRUE install

## Webhook between github -> jenkins
**Jenkins side:**
-------------
1- install "github integration plugin" in jenkins
2- in jenkins job> build triggers : check the github hook option


in Github side:
---------------
1- edit the github repository the go to setting
2- click button "add webhook"
3- in the payload URL fill "jenkins URL/github-webhook/" ex:"xx.xx.xx.xx:8080/github-webhook/".
please don't forget the last "/" in this URL as it is mandatory.
4- change content type to "application-json"
5- click the radio button "just the push event"
