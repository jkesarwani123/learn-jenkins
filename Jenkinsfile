pipeline {
    agent {
    node{
     label 'workspace'
     }
    }
    options {
        ansiColor('xterm')
    }
    parameters {
        string(name: 'PERSON', defaultValue: 'staging', description: '')
    }
    environment {
    SAMPLE ="JK"
    }
    stages {
     stage('One') {
        steps {
            sh 'echo Hello World'
            sh 'echo ${SAMPLE}'
            sh 'echo ${PERSON}'
        }
     }
    }
    post {
        always {
         sh 'echo close cleanup'
        }
    }
    }