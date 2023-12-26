pipeline{
  agent{
    label('built-in')
    customWorkspace "/mnt"
  }
  stages{
    stage('stage1'){
      steps{
       // sh "sudo yum install git -y"
        sh "git clone https://github.com/Aniruddha-22-git/new-repo.git"
        sh "cp -r /mnt/new-repo/sample.war /mnt/servers/apache-tomcat-9.0.84/webapps/
        //sh "sudo service httpd start "
        //sh "sudo cp -r /mnt/index/index.html /var/www/html/"
        //sh "sudo chmod -R 777 /var/www/html"
        sh "chmod -R 777 /mnt/servers/apache-tomcat-9.0.84/webapps/sample.war"
        sh "./startup.sh /mnt/servers/apache-tomcat-9.0.84/bin"
      }
    }
  }
}
