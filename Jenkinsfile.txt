pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build du projet'
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello World depuis Jenkins CI/CD'
            }
        }
    }
}
