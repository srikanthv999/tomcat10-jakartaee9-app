pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                
              
                sh 'mvn clean install'
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
                sh 'sudo cp /var/lib/jenkins/.m2/repository/example/demo/helloworld/1.0-SNAPSHOT/helloworld-1.0-SNAPSHOT.war /opt/apache-tomcat-9.0.72/webapps/'
            }
        }
    }
}
