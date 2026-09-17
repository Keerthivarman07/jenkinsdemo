pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                bat 'javac calculator.java'
            }
        }

        stage('Run') {
            steps {
                bat 'echo 20 5 | java calculator'
            }
        }
    }

    post {
        success {
            echo 'Build Successful'
        }

        failure {
            echo 'Build Failed'
        }
    }
}