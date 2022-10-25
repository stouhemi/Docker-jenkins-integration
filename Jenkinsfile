node{
  stage('SCM Checkout'){
    
    git 'https://github.com/stouhemi/Docker-jenkins-integration'
  }
  
  stage('Compile-package'){
    def mvnHome = tool name: 'maven-3.8.6', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  
  stage('email notification'){
    mail bcc: '', body: '''Hi welcome to jenkins email alerts
    Thanks
    Seif
    ''', cc: '', from: '', replyTo: '', subject: 'job jenkins', to: 'seiftouhemi@gmail.com'
  
  }
}
