pipeline{
  agent{
    label('slave-1')
    
  }
  stages{
    stage('stage1'){
      steps{
        //sh "sudo yum install git -y"
       /* sh "sudo git clone https://github.com/Aniruddha-22-git/index.git /mnt/index"
        sh "sudo yum install httpd -y"
        sh "sudo service httpd start "
        sh "sudo cp -r /mnt/index/index.html /var/www/html/"
        sh "sudo chmod -R 777 /var/www/html"*/
        sh "sudo wget https://github.com/AKSarav/SampleWebApp/raw/master/dist/SampleWebApp.war "
        //sh "sudo cp -r /SampleWebApp.war /mnt/servers/apache-tomcat-9.0.84/webapps"
        //sh "sudo  chmod -R 777 /mnt/servers/apache-tomcat-9.0.84/webapps/SampleWebApp.war"
        //sh "sudo cd /mnt/servers/apache-tomcat-9.0.84/bin/ && ./startup.sh"
      }
    }
  }
}
