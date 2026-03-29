pipeline {
    agent any

    stages {

        stage('Build Image') {
            steps {
                script {
                    sh 'docker build -t myapp .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run -d -p 5000:5000 myapp'
                }
            }
        }
    }
}