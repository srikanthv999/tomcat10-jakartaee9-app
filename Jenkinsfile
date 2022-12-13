pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage'
                sh 'mvn clean compile'
                }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy'
                }
         }
         stage('Test') {
            steps {
                echo 'Test'
            }
        }
    }
}
