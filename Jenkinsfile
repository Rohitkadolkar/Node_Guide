pipeline{
  agent {label 'dev-agent'}
  stages {
    stage ('build'){
      steps {
        echo "Building and testing ..."
        sh 'docker build -t node-guide:latest'
      }
    }
    stage ('Deploy' {
      steps {
        sh 'docker run -d -p 3000:3000 node-guide:latest
