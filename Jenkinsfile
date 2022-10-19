pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                sh 'echo hey'
            }
        }
        stage('coaching') {
            agent { label 'jenkins' }
            steps {
                git url: 'https://github.com/ratnakarchitti/game-of-life.git',
                    branch: 'master'
            }
        }
    }
}













