pipeline {
    agent any

    tools {
        maven 'Maven-3' 
        nodejs 'NodeJS-25'
    }

    stages {
        stage('Build Backend (Java)') {
            steps {
                // On dit à Jenkins d'entrer dans le dossier backend
                dir('backend') {
                    sh 'mvn clean package -DskipTests'
                }
            }
        }
        
        stage('Build Frontend (React)') {
            steps {
                // On dit à Jenkins d'entrer dans le dossier frontend
                dir('frontend') {
                    sh 'npm install'
                    sh 'npm run build'
                }
            }
        }
        
        stage('Déploiement sur le NAS') {
            steps {
                echo 'Ici on copiera les fichiers vers Web Station et on relancera le Docker Java !'
            }
        }
    }
}