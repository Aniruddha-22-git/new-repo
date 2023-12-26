pipeline{
  agent{
    label {
      label ('built-in')
    customWorkspace "/mnt/host"
  }
  }
  stages{
    stage('stage1'){
      steps{
        //sh "git clone https://github.com/Aniruddha-22-git/new-repo.git"
       // sh "cp -r /mnt/host/sample.war /mnt/servers/apache-tomcat-9.0.84/webapps/"
       // sh "chmod -R 777 /mnt/servers/apache-tomcat-9.0.84/webapps/sample.war"
        sh "cd /mnt/servers/apache-tomcat-9.0.84/bin/ && ./startup.sh"
      }
    }
  }
}
