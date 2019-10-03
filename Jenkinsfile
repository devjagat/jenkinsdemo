pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Building Stage" 
            }
        }
        stage('Test') { 
            steps {
                echo "Testing Stage" 
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deploying Stage" 
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'Thank You for using Development Branch !!'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
