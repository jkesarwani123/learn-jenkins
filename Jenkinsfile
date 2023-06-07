pipeline {
    agent {
    node{
     label 'workspace'
     }
    }
    environment {
    SAMPLE ="JK"
    }
    stages {
     stage('One') {
        steps {
            sh 'echo Hello World'
            sh 'echo ${SAMPLE}''
        }
     }
    }
    post {
        always {
         sh 'echo close cleanup'
        }
    }
    }