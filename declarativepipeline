pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                sh 'echo hello'
            }
        }
        stage('learning') {
            agent { label 'OPENJDK-11-MAVEN' }
            steps {
                git url: 'https://github.com/kundan-1234567/scripted-pipeline.git', 
                    branch: 'master'
            }
        }
    }
}

