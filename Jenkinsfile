node('UBUNTU') {
    stage('VCS') {
         git 'https://github.com/pradeepballa/jenkinsbuildpractic.git'
     }
     
    stage('package'){
        sh 'mvn package'
    }
    stage('Artifacts'){
        archiveArtifacts 'gameoflife-web/target/*.war'
    }

}