pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Check out your source code from version control
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Example for Maven build
                sh 'mvn clean install'

                // Or, if you're using Gradle
                // sh 'gradle build'
            }
        }
    }

    post {
        success {
            echo 'Build successful! Deploy your application or perform additional steps here.'
        }
        failure {
            echo 'Build failed! Take necessary actions for failure.'
        }
    }
}
