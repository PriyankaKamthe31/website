pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/PriyankaKamthe31/website.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project"
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}
