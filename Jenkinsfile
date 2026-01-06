pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Bhavin2123/jenkins-ci-cd-project.git'
            }
        }
        stage('Build & Deploy') {
            steps {
                sh '''
                chmod +x app.sh
                ./app.sh
                '''
            }
        }
    }
}

