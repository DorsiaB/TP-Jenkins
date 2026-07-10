pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Compilation du projet Maven'
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Execution des tests Maven'
                sh 'mvn test'
            }
        }
    }
}