pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'E:\\2CSil\\OUTILS\\gradle-4.10.2-all\\gradle-4.10.2\\bin\\gradle build'
      }
    }
    stage('Mail Notification ') {
      steps {
        mail(subject: 'Jenkins', body: 'soit echec ou réussite de l\'intégration ')
      }
    }
  }
}