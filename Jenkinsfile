pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project'
                sh './gradlew clean build -x test'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the project'
                sh './gradlew clean test'
            }
        }
        stage('Deploy') {
            when {
                expression {env.GIT_BRANCH == 'origin/main'}
            }
            steps {
                echo 'Deploying the project'
            }
        } 

        stage('ProdDeploy') {
             when {
                expression {env.GIT_BRANCH == 'origin/main'}
            }
            steps {
                echo 'Deploying the project'
            }
        }
    }
}
