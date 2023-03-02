pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage'
                sh '/opt/apache-maven-3.9.0/bin/mvn clean install'
                }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy'
                sh 'sudo cp /var/lib/jenkins/.m2/repository/example/demo/helloworld/1.0-SNAPSHOT/helloworld-1.0-SNAPSHOT.war /opt/tomcat/apache-tomcat-10.0.27/webapps/'
                }
         }
         stage('Test') {
            steps {
                echo 'Test'
            }
        }
    }
}
