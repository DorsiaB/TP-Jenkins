pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Compilation du projet Maven'
                sh '''
                cd TP2/projet-maven
                /var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/Maven-3.9.16/bin/mvn clean package
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Execution des tests Maven'
                sh '''
                cd TP2/projet-maven
                /var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/Maven-3.9.16/bin/mvn test
                '''
            }
        }
    }
}