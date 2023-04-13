pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage automatically'
                sh 'mvn clean install'
                }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy'
                sh 'sudo cp /var/lib/jenkins/.m2/repository/example/demo/helloworld/1.0-SNAPSHOT/helloworld-1.0-SNAPSHOT.war /opt/apache-tomcat-9.0.72/webapps/'
                }
         }
         stage('Test') {
            steps {
                echo 'Test'
            }
        }
    }
}
