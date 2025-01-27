pipeline {
    // agent any
    // agent { label 'labelName' }
    agent { node { label 'agent-1' } }
    stages {
        stage('Build-1') {
            steps {
                echo "build"
            }
        }
        stage('Test-1') {
            steps {
                echo "test"
            }
        }
        stage('Deploy-1') {
            steps {
                echo "deploy"
            }
        }
    }
}