pipeline {
    agent {
      label 'agent1'
    }
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Compile') {
            steps {
                script {
                    sh 'javac App.java'
                }
            }
        }
        
        stage('Run') {
            steps {
                script {
                    sh 'java App'
                }
            }
        }
    }
}
