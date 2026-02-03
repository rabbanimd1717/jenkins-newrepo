pipeline {
    agent {
        label 'AGENT-1'
    }

    options {
        timeout(time: 1 , unit: 'HOURS')
        disableConcurrentBuilds()
    }
    

    stages {
        stage('Build') {
            steps {
                sh 'echo This is build stage'
            }
        }
        stage('Test') {
            steps {
                sh 'echo This is test stage'
                sleep 10
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo This is deploy stage'
            }
        }
    }
}