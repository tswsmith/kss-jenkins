pipeline {
  agent any
  stages {
    stage('aage badhe?') {
      steps {
        input(message: 'chale?', id: 'kon', ok: 'yes')
      }
    }
    stage('Git checkout') {
      steps {
        git(url: 'https://github.com/tswsmith/kss-jenkins.git', branch: 'master', changelog: true, poll: true, credentialsId: 'tswsmith')
      }
    }
    stage('test') {
      steps {
         withEnv(["PATH+MAVEN=${tool 'maven4'}/bin"]) {
          sh "mvn test"
        }
      }
    }
  }
}
