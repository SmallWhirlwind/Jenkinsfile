node {
    stage('Download Project') {
        git 'https://github.com/SmallWhirlwind/Jenkinsfile.git'
    }
    stage('Copy Webpage to Nginx') {
        sh '''
        sudo rm /home/webpage/index.html
        sudo cp index.html /home/webpage'''
    }
    stage('Restart Nginx') {
        sh '''sudo nginx -s reload'''
    }
}
