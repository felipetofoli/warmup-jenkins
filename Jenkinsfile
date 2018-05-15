pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Iniciando build'
        sh 'mvn clean package'
      }
    }
    stage('test') {
      steps {
        echo 'Iniciando testes'
        sh 'mvn test'
      }
    }
  }
  environment {
    agent = 'master'
  }
}