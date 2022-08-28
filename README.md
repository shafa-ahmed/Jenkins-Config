# Jenkins-Config
#Complete Configuration of Jenkins Console
#Author:- Shafa Ahmed [+91-9718320763] [shafaahmed100@hotmail.com / shafamalick82@gmail.com]
Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing,and deploying, facilitating continuous integration and continuous delivery.

#install the java packages
Yum install java* -y

#disable the security linux
setenforce 0

#install the jenkins packages
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key

#install the jenkins
yum install Jenkins* -y

systemctl restart Jenkins
systemctl enable Jenkins
systemctl status Jenkins

#port number verification
ps -ef | grep java
netstat -lntp | grep 6262

#Go to the security and add browsing enable on port number 8080
#copy the public IP and with colon 8080, browse it


