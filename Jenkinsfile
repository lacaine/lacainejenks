pipeline{
    agent any
    stages{
        stage('1-clone'){
            steps{
             checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-id', url: 'https://github.com/lacaine/lacainejenks.git']])  
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