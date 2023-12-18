Create a .sh file and paste all below command in it and save it.

##Install extra packege enterprices linux using below command##
      
       amazon-linux-extras install epel 

##Java install command##

    amazon-linux-extras install java-openjdk11

##Jenkins repo add. ##


    sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
    sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key

##install jenkins.##


    yum install jenkins

service jenkins start

Run the .sh file 
jenkins will get installed successfully.


