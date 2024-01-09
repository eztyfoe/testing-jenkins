pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo 'Test Success.'
            }
        }
    }

    post {
        success {
            echo 'Test successful! Take any necessary actions for success.'
        }
        failure {
            echo 'Test failed! Take any necessary actions for failure.'
        }
    }
}
