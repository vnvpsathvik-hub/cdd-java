pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                bat 'javac code.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java code'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check errors above.'
        }
    }
}


