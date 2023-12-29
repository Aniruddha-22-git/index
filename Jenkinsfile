pipeline{
  agent{
    label{
      label "slave-1"
    customWorkspace "/mnt/23q1"
    }
  }
  stages{
    stage('stage1'){
      steps{
        sh "sudo cp -r /mnt/23q1/index.html /var/www/html"
        sh "sudo service httpd start "

      }
    }
  }
}
