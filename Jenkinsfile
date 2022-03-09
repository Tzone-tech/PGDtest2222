pipeline{
    agent any
    stages{
        stage('GIT Clone'){
            steps{
                sh 'mkdir PGDtest222'
                git  'https://github.com/Tzone-tech/PGDtest2222.git'
                
            }
        }
        stage('Test'){
            steps{
                // sh "mkdir Tonytestphase"
                sh "cp PGDtest222 Tonytestphase"
            }
        }
    }
}
