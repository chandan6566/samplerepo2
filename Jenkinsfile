pipeline{
    agent any
    stages{
        stage('Memory Usage'){
            steps{
                sh 'echo "htop"'
            }
        }
        stage('Disk Usage'){
            steps{
                sh 'echo "df -h"'
            }
        }
    }
}
