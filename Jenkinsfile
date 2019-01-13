pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'gradle build'
      }
    }
    stage('Mail Notification ') {
      steps {
        mail(subject: 'Jenkins', body: 'soit echec ou réussite de l\'intégration ')
      }
    }
  }
}