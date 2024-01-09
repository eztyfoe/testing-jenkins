pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo 'This is a test stage. You can add your test commands here.'
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
