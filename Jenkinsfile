pipeline {
  agent any
  
  stages {

    stage('Build Release') {
      when {
        branch 'master'
      }
      echo "Aqui ando perro"
    }

    stage('Promote to Environments') {
      when {
        branch 'master'
      }
      echo "Aqui tambien"
    }
  }

  post {
    always {
      cleanWs()
    }
  }
}
