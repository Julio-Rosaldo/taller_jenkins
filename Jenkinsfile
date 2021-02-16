pipeline {
  agent any
  stages {
    stage('Hola_mundo') {
      steps {
        echo 'Hola Mundo'
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