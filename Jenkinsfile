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

    stage('Despedida') {
      steps {
        input(message: 'Ya termino el taller', ok: 'Buen taller')
      }
    }

  }
  environment {
    Nombre = 'Julio'
  }
}