node{
  stage('SCM Checkout'){
    git 'https://github.com/stouhemi/Docker-jenkins-integration'
  }
  
  stage('Compile-package'){
    sh 'mvn package'
  }
}
