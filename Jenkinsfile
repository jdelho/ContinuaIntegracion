pipeline {
    agent any

    stages {
        stage("Proceso") {
            steps {
                script {
                    ejecutarProceso()
                }
            }
        }
    }
}

def ejecutarProceso () {
    if (new Date().getHours() > 12) {
        echo "El proceso puede ejecutarse"
        wrap([$class: 'BuildUser']) {
          sh 'echo "${BUILD_USER}"'
        }
    } else {
        echo "El proceso no puede ejecutarse"
    }
}
