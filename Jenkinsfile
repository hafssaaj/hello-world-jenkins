pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Code récupéré depuis Git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Étape de build simulée'
                // Pour un projet web, on peut juste vérifier les fichiers
                sh 'ls -la'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Exécution des tests simulée'
                // Exemple simple de test
                sh 'echo "Tests passés avec succès"'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Déploiement simulé'
                sh 'echo "Application déployée avec succès!"'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline terminé avec succès!'
        }
        failure {
            echo 'Pipeline échoué!'
        }
    }
}