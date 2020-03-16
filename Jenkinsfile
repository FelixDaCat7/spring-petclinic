pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat './mvnw package'
        bat 'mvn clean test package'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing'
      }
    }

    stage('Package') {
      steps {
        echo 'Packaging'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}