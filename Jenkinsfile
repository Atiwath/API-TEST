pipeline {
    agent any
    stages {
        stage('version') {
            steps {
                echo 'Running Python version:'
                sh 'python --version'
            }
        }
        stage('hello') {
            steps {
                echo 'Hello, World!'
            }
        }
    }
}
