pipeline{
    agent none
    
    stages{
        stage('Front End'){
            agent{
                docker { image 'cloudstack/marvin' }
            steps{
                sh 'mvn --version'
            }
        }
    }
        stage('Backend'){
            agent{
                docker {image 'node:16-latest' }
            }
            steps{
                sh 'node --version'
            }
    }
}
}
