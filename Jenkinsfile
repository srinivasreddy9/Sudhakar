pipeline {
    agent any
stages{
stage('SCM Checkout'){
  git credentialsId: 'GITCREDENTIALS', url: 'https://github.com/srinivasreddy9/simple-app.git'
        
    }
    tools {
  maven 'Maven-3.6.1'
}
stages{
    stage('Build'){
        steps{
            sh 'mvn clean package'
        }
    }
}
}
