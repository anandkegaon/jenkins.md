### How to Install Jenkins on Ubuntu ##

## Update the packages to their latest versions available after a fresh install of Ubuntu ##
    sudo apt-get update -y && sudo apt-get upgrade -y 

## To install Java OpenJDK 11, execute the following command ##
    sudo apt install openjdk-11-jdk -y 

## To check the installed Java version, execute the following command ##
     java --version 

## we will add the Jenkins repository and Key since they are not added by default in Ubuntu ##
     curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null 

      echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null 

  ## Update the system and install Jenkins ##
     sudo apt update -y 
     sudo apt install jenkins -y 


 ## Once installed, start and enable the Jenkins service ##
     sudo systemctl start jenkins && sudo systemctl enable jenkins 

 ## To check the status of the service ##
     sudo systemctl status jenkins 
 
## browse the jenkins using 
    http://localhot:8080 

## Copy the intial admin password form the below location and paste it ##
    cat /var/lib/jenkins/secrets/initialAdminPassword 

 Finally Jenkins get started.
## Create a .sh file and paste this below code and run that file so that all command will get execute one by one.

    sudo apt-get update -y && sudo apt-get upgrade -y
    sudo apt install openjdk-11-jdk -y
    curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null 
    echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null 
    sudo apt update -y 
    sudo apt install jenkins -y 
    sudo systemctl start jenkins && sudo systemctl enable jenkins 
    sudo systemctl status jenkins
    
   

 
 
