pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'flutter pub get'
            }
        }

        stage('Test') {
            steps {
                bat 'flutter test'
            }
        }

        stage('Build Web') {
            steps {
                bat 'flutter build web --release'
            }
        }
    }
}