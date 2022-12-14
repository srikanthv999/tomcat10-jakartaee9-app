pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage'
                sh 'mvn clean install'
                }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy'
                sh 'cp /var/lib/jenkins/.m2/repository/example/demo/helloworld/1.0-SNAPSHOT/helloworld-1.0-SNAPSHOT.war /opt/tomcat/apache-tomcat-10.0.27/webapps/'
                }
         }
         stage('Test') {
            steps {
                echo 'Test'
            }
        }
    }
}
