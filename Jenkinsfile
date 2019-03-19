pipeline {
    agent { docker { image 'python:3.6.8' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
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
}
