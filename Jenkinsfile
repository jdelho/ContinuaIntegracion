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
            echo "Usuario: $BUILD_USER"
            echo "Id Usuario: $BUILD_USER_ID"
        }
        echo "Version Java:" 
        bat "java -version"
    } else {
        echo "El proceso no puede ejecutarse"
    }
}
