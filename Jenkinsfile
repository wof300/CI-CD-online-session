pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        script {
          checkout scm







          def customImage = docker.build("${registry}:${env.BUILD_ID}")
        }

      }
    }

  }
  environment {
    registry = 'wof300/cicdrepo'
  }
}