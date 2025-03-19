pipeline {
  agent any
  tools { 
      maven 'DHT_MVN' 
      jdk 'DHT_SENSE' 
  }

  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/ivanyang02/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
  tools {
    maven 'Maven'
    jdk 'Java 8'
  }
}
