pipeline {
  agent {
    docker {
      image 'maven:3.8.6-openjdk-11-slim'
    }
  }
  triggers {
   cron 'H  *  *  *  *'
  }
  stages {
    stage('build') {
      steps {
        sh 'mvn --batch-mode --update-snapshots verify'
      }
    }

  }
}
