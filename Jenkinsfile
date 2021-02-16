pipeline {
  agent any
  stages {
    stage('Hola_mundo') {
      steps {
        echo 'Hola Julio'
        bat(script: 'echo %PATH%', returnStdout: true)
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'salida.txt', text: 'Mensaje de salida')
        archiveArtifacts '*.txt'
      }
    }

  }
  environment {
    Nombre = 'Valor'
  }
}