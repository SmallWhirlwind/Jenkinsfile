pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    options {
        buildDiscarder(logRotator(numToKeepStr: '7'))
    }

    stages {
        stage('Copy Webpage to Nginx') {
            steps {
                sh 'cp helloWorld.html /home/webpage'
            }
        }
        stage('Restart Nginx') {
            steps {
                sh 'sudo nginx -s reload'
            }
        }
    }
}
