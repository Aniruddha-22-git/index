pipeline{
  agent{
    label{
      label "slave-1"
   // customWorkspace "/mnt/slave1"
    }
  }
  stages{
    stage('stage1'){
      steps{
        sh "sudo yum install git -y"
        sh "sudo rm -rf /mnt/index"
        sh "sudo git clone https://github.com/Aniruddha-22-git/index.git /mnt/index"
        sh "sudo yum install httpd -y"
        sh "sudo service httpd start "  
        sh "sudo cp -r /mnt/index/index.html /var/www/html/"
        sh "sudo chmod -R 777 /var/www/html"
        sh "sudo rm -rf /mnt/servers"
        //sh "sudo wget -P /https://github.com/AKSarav/SampleWebApp/raw/master/dist/SampleWebApp.war  "
        sh "sudo mkdir /mnt/servers"
        //sh "sudo cd /mnt/servers"
        sh "sudo wget -P /mnt/servers https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.105/bin/apache-tomcat-9.0.105.zip"
        sh "sudo cd /mnt/servers"
        sh "sudo unzip /mnt/servers/apache-tomcat-9.0.105.zip -d /mnt/servers/"
        sh "sudo chmod -R 777 /mnt/servers/apache-tomcat-9.0.105"
        sh "sudo wget -P /mnt/servers/apache-tomcat-9.0.105/webapps https://tomcat.apache.org/tomcat-6.0-doc/appdev/sample/sample.war"
        //sh "sudo cp -r /mnt/slave1/SampleWebApp.war /mnt/slave1/servers/apache-tomcat-9.0.84/webapps"
        sh "sudo  chmod -R 777 /mnt/servers/apache-tomcat-9.0.105/webapps/sample.war"
     //sh "sudo yum install httpd -y "
        sh "sudo /mnt/servers/apache-tomcat-9.0.105/bin/startup.sh"
      }
    }
  }
}
