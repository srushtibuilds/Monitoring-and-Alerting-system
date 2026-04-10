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
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python test.py'
            }
        }

        stage('Build Success') {
            steps {
                sh 'echo "Monitoring System Build Successful!"'
            }
        }

    }
}
