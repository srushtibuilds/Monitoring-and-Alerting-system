pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                bat 'python -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat 'python test.py'
            }
        }

        stage('Done') {
            steps {
                bat 'echo Build Successful'
            }
        }

    }
}
