pipeline {
    // agent any
    agent { label 'agent-1' }
    // agent { node { label 'agent-1' } }
    // NOTE: agent { node { label 'labelName' } } behaves the same as agent { label 'labelName' }, but node allows for additional options (such as customWorkspace).
    // agent {
    //     node {
    //         label 'agent-1'
    //         customWorkspace '/tmp'
    //         }
    // }

    
    stages {
        stage('Build-1') {
            steps {
                echo "build on webhook"
            }
        }
        stage('Test-1') {
            steps {
                echo "test on webhook agent-1"
            }
        }
        stage('Deploy-1') {
            steps {
                echo "deploy on agent-1"
                
            }
        }
    }

    post { 
        always { 
            echo 'run always'
        }
        success { 
            echo 'run only after success'
        }
        failure { 
            echo 'run only after failure'
        }
    }
}