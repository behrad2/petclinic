pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      steps {
        sh 'mvn clean'
      }
    }

    stage('test') {
      agent any
      steps {
        sh 'mvn test'
      }
    }

    stage('deploy') {
      agent any
      steps {
        sh 'mvn package'
      }
    }

  }
  environment {
    stage = ''
  }
}