pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat './mvnw package'
				bat 'mvn clean test package'
            }
        }
    }
}
