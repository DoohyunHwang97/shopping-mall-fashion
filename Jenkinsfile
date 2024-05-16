pipeline {
  agent any
  environment {

    }

    stage('Test') {
        steps {
            sh './gradlew test'
            echo 'test success'
        }
    }

    stage('Build') {
      steps {
           sh './gradlew clean build --exclude-task test --exclude-task asciidoctor'
           echo 'build success'
      }
    }
  }
}