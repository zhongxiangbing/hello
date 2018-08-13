pipeline {
  agent any
  stages {
    stage('package') {
      agent any
      steps {
        sh 'mvn clean install'
      }
    }
  }
}