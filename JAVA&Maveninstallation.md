Step 1: Download the JDK Binaries:

Go to the URL: https://jdk.java.net/13/ Copy the download link for Linux/x64 build. 
Then use the below command to download and extract it.


    wget https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz
    tar -xvf openjdk-13.0.1_linux-x64_bin.tar.gz
     mv jdk-13.0.1 /opt/
 I have moved JDK to /opt, you can keep it anywhere in the file system.    

 Step 2: Setting JAVA_HOME and Path Environment Variables :

 Open .profile file from the home directory and add the following lines to it.

     JAVA_HOME='/opt/jdk-13.0.1'
     PATH="$JAVA_HOME/bin:$PATH"
     export PATH

  Step 3: Verify the Java Installation :

  You can run java -version command to verify the JDK installation.

     java -version


  Step 4: Download the Maven Binaries :

  Go to the URL: https://maven.apache.org/download.cgi Copy the link for the “Binary tar.gz archive” file.
  Then run the following commands to download and untar it.

     wget https://mirrors.estointernet.in/apache/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz
     tar -xvf apache-maven-3.6.3-bin.tar.gz
     mv apache-maven-3.6.3 /opt/


  Step 5: Setting M2_HOME and Path Variables :
     
     M2_HOME='/opt/apache-maven-3.6.3'
     PATH="$M2_HOME/bin:$PATH
     export PATH
 STEP 6 "Verify Maven Installation

     mvn -version

  That's it.  
