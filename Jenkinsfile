properties([pipelineTriggers([pollSCM('* * * * *')])])
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Print all files') {
            steps {
                sh 'ls -ltr'
            }
        }
        stage('Execute python') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
