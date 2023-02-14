pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o hello ./main/hello0.cpp '
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
