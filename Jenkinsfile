pipeline{
    agent any
    stages{
        stage('GIT Clone'){
            steps{
                // sh 'mkdir PGDtest222'
                git  'https://github.com/Tzone-tech/PGDtest2222.git'
                
            }
        }
  agent {
    kubernetes {
        label podlabel
        yaml """
kind: Pod
metadata:
  name: jenkins-agent
spec:
  containers:
  - name: kaniko
    image: nginx 2.0.0
    imagePullPolicy: Always
        
"""
        }
    }
        stage('Test'){
            steps{
                 sh "mkdir Tonytestphase"
                sh "cp -r PGDtest222 Tonytestphase"
            }
        }

    }
}
