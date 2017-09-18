node {
    stage('Copy Webpage to Nginx') {
        sh 'cp helloWorld.html /home/webpage'
    }
    stage('Restart Nginx'') {
        sh 'sudo nginx -s reload'
    }
}
