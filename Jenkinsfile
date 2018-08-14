pipeline {
  agent any
  stages {
    stage('package') {
      agent any
      steps {
        sh 'mvn clean install'
      }
    }
    stage('write') {
      steps {
        writeFile(file: 'dockerfile', text: 'FROM aaa \\n COPY a /a', encoding: 'utf -8')
      }
    }
  }
}