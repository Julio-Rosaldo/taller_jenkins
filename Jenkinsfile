pipeline {
  agent any
  stages {
    stage('Hola_mundo') {
      steps {
        echo 'Hola Julio'
        bat 'SET'
        bat 'echo %Nombre%'
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
    Nombre = 'Julio'
  }
}