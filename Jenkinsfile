pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                bat 'py -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat 'py test.py'
            }
        }

        stage('Done') {
            steps {
                bat 'echo Build Successful'
            }
        }

    }
}
