pipeline{
  agent{
    label('built-in')
  }
  stages{
    stage('stage1'){
      steps{
        sh "git clone https://github.com/Aniruddha-22-git/index.git /mnt"
        sh "yum install httpd -y"
        sh "service httpd start "
        sh "cp /mnt/index/index.html /var/www/html"
        sh "chmod -R 777 /var/www/html"
        
        //sh "yum install docker -y "
        //sh "systemctl start docker"
        //sh "systemctl enable docker"
      //sh "git clone https://github.com/Aniruddha-22-git/docker1.git -b 23q1 /mnt/23q1"
    //    sh "docker run -itdp 80:80 --name 23q1 httpd"
  //      sh "docker cp /mnt/23q1/index.html 23q1:/usr/local/apache2/htdocs"
//        sh "docker exec 23q1 chmod -R 777 /usr/local/apache2/htdocs"
      }
    }
  }
}
