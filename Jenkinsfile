pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                bat '''
                "C:\\Users\\Srushti\\AppData\\Local\\Python\\pythoncore-3.14-64\\python.exe" -m pip install -r requirements.txt
                '''
            }
        }

        stage('Test') {
            steps {
                bat '''
                "C:\\Users\\Srushti\\AppData\\Local\\Python\\pythoncore-3.14-64\\python.exe" test.py
                '''
            }
        }

        stage('Done') {
            steps {
                bat 'echo Build Successful'
            }
        }

    }
}
