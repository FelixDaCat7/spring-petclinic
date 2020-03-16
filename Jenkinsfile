pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat './mvnw package'
        bat 'mvn clean'
      }
    }

    stage('Test') {
      steps {
        bat 'mvn test'
      }
    }

    stage('Package') {
      steps {
        bat 'mvn package'
      }
    }

    stage('Deploy') {
    when{ branch 'master' }
	  steps {
        echo 'Deploy'
      }
    }

  }
}