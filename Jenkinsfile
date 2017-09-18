node {

  stage ('Download Code') {
    git 'https://github.com/phodal/growth-studio'
  }

  stage ('Copy Webpage to Nginx') {
    sh './ci/setup.sh'
  }

  stage ('Restart Nginx') {
    sh './ci/install.sh'
  }
}