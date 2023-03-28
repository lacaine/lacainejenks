pipeline{
    agent any
    stages{
        stage('1-clone'){
            steps{
            }
        }
        stage('2-systemscheck'){
            steps{
                sh 'sudo systemctl status jenkis'
            }
        }
        stage ('3-diskcheck'){
            steps{
                sh 'df -h'
            }
        }
        stage ('4-blockcheck'){
            steps{
                sh 'lsblk'
            }
        }
    }
}