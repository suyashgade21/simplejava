pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/suyashgade21/simplejava.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Show WAR') {
            steps {
                sh 'ls -lh target/'
            }
        }
    }
}