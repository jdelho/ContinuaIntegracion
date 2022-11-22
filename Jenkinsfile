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
            def user = env.BUILD_USER_ID
            println user
        }
    } else {
        echo "El proceso no puede ejecutarse"
    }
}
