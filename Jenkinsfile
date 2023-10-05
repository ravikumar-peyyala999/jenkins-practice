pipeline {
    agent any { node { label 'agent-1' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo 'always run if job is success or failure...'
        }
        success {
            echo 'run if job is success...'
        }
        failure {
            echo 'run if job is failure...'
        }
    }
}