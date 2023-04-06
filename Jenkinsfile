properties([pipelineTriggers([pollSCM('30 * * * *')])])
pipeline {
    agent any

    stages {
        stage('wellcom') {
            steps {
               checkout scm
               sh 'python NewScreen/main.py'
            }
        }
        stage('clicks') {
            steps {
               checkout scm
               sh 'python NewButtons/main.py'
            }
        }
    }
}
