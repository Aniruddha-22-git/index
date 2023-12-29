pipeline{
  agent{
    label{
      label "slave-1"
    customWorkspace "/mnt/slave1"
    }
  }
  stages{
    stage('stage1'){
      steps{
        //sh "sudo yum install git -y"
       // sh "sudo git clone https://github.com/Aniruddha-22-git/index.git /mnt/index"
        //sh "sudo yum install httpd -y"
        //sh "sudo service httpd start "
        //sh "sudo cp -r /mnt/slave1/index.html /var/www/html/"
       // sh "sudo chmod -R 777 /var/www/html"
       // sh "sudo wget https://github.com/AKSarav/SampleWebApp/raw/master/dist/SampleWebApp.war  "
       // sh "sudo mkdir servers"
        sh "sudo cd /mnt/slave1/servers"
        sh "wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.84/bin/apache-tomcat-9.0.84.zip /mnt/slave1/servers"
        //sh "cd /mnt/slave1/servers"
        //sh "unzip apache-tomcat-9.0.84.zip "
        //sh "sudo chmod -R 777 apache-tomcat-9.0.84"
        //sh "sudo cp -r /mnt/slave1/SampleWebApp.war /slave1/servers/apache-tomcat-9.0.84/webapps"
        //sh "sudo  chmod -R 777 /mnt/slave1/servers/apache-tomcat-9.0.84/webapps/SampleWebApp.war"
        //sh "sudo cd /mnt/slave1/servers/apache-tomcat-9.0.84/bin/ && ./startup.sh"
      }
    }
  }
}
