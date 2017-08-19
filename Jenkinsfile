pipeline {
  agent any
  stages {
    stage('aage badhe?') {
      steps {
        input(message: 'chale?', id: 'kon', ok: 'yes')
      }
    }
    stage('Git se kheech') {
      steps {
        git(url: 'https://github.com/tswsmith/kss-jenkins.git', branch: 'kss-jenkins', changelog: true)
      }
    }
    stage('test') {
      steps {
        tool(name: 'maven4', type: 'maven')
        sh 'mvn test'
      }
    }
  }
}