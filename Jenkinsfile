pipeline {
    agent any

    stages {
        stage('Construction') {
            steps {
                echo 'Construction du projet...'
                // Ajoutez ici les étapes de construction, par exemple :
                sh 'mvn clean package' // Commande Maven pour construire le projet
            }
        }

        stage('Test') {
            steps {
                echo 'Exécution des tests...'
                // Ajoutez ici les étapes de test, par exemple :
                sh 'mvn test' // Commande Maven pour exécuter les tests
            }
        }

        stage('Déploiement') {
            steps {
                echo 'Déploiement de l\'application...'
                // Ajoutez ici les étapes de déploiement, par exemple :
                sh 'scp target/*.jar user@server:/path/to/deploy' // Déployer le fichier JAR sur le serveur
            }
        }
    }
}
