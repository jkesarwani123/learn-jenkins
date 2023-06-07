pipeline {
    agent {
    node{
     label 'workspace'
     }
    }
    stages {
     stage('One') {
        steps {
            sh 'echo Hello World'
        }
     }
    }
    post {
        always {
         sh 'echo close cleanup'
        }
    }
    }