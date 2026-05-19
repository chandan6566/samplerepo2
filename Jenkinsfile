pipeline {
    agent none  // No global agent; each stage uses its own Docker container
    
    stages {
        stage('Front End) {
            agent {
                docker { image 'maven:3.9.2-openjdk-17' } // Maven + Java preinstalled
            }
            steps {
                sh 'mvn --version'
            }
        }
        
        stage('Backend') {
            agent {
                docker { image 'node:16-latest' } // Node.js preinstalled
            }
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }
}
