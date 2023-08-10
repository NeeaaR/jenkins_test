pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                // Cloner le dépôt (ceci est implicite si vous utilisez une source de code intégrée à Jenkins)
                checkout scm
            }
        }

        stage('Test') {
            steps {
                // Exécutez un script de test fictif. Adaptez ceci selon ce que vous avez dans votre dépôt.
                sh './test_script.sh'
            }
        }

        stage('Build') {
            steps {
                // Exécutez un script de construction fictif. Adaptez ceci selon ce que vous avez dans votre dépôt.
                sh './build_script.sh'
            }
        }
    }

    post {
        success {
            echo "Les étapes se sont terminées avec succès!"
        }
        failure {
            echo "Une étape a échoué."
        }
    }
}
