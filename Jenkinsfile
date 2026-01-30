pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                sh 'javac code.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java code'
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
