pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'gradle build'
        sh 'gradle javadoc'
        sh 'gradle jar'
      }
    }
    stage('Mail Notification ') {
      steps {
        mail(subject: 'Jenkins', body: 'soit echec ou r�ussite de l\'int�gration ')
      }
    }
  }
}