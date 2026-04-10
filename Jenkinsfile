pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                git 'https://github.com/srushtibuilds/Monitoring-and-Alerting-system.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'python test.py'
            }
        }

        stage('Success') {
            steps {
                bat 'echo Build Successful!'
            }
        }

    }
}
