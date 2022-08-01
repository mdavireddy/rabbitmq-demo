pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the project'
            }
        }
        stage('Deploy') {
            when {
                branch "master"
            }
            steps {
                echo 'Deploying the project'
            }
        }

        stage('Deploy') {
             when {
                branch "master"
            }
            steps {
                echo 'Deploying the project'
            }
        }
    }
}