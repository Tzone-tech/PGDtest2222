pipeline{
    agent any
    stages{
        stage('GIT Clone'){
            steps{
                git  'https://github.com/Tzone-tech/PGDtest2222.git'
            }
        }
        stage('Test'){
            steps{
                sh "mkdir Tonytestphase"
                sh "cp PGDtest2222 Tonytestphase"
            }
        }
    }
}
