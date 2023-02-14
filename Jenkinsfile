pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o hello hello.cpp '
            }
        }
        stage('Test') {
            steps {
                sh './hello '
            }
        }

    }

    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
