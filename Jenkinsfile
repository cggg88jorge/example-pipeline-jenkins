pipeline {
  agent any

  stages {

    stage('checkout') {
      when {
        branch 'master'
      }
      steps{
        checkout scm
      }
    }

    stage('Build Release') {
      when {
        branch 'master'
      }
      steps{
        echo "Aqui ando perro"
      }
    }

    stage('Promote to Environments') {
      when {
        branch 'master'
      }
      steps{
        echo "Aqui tambien"
      }
    }
  }

  post {
    always {
      cleanWs()
    }
  }
}
