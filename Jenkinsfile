pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                // sh 'git clone https://github.com/siva8143kumar/basic-jsp-example.git'
              
                sh '/opt/apache-maven-3.9.0/bin/mvn clean install'
                sh 'ls -lrt'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
