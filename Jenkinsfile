def clima = "Lluvia"
def cantidadHabitantes = 3000
def numero2 = 2
pipeline {
    agent any

    stages {
        stage("Clima") {
            steps {
                println clima
            }
        }
        stage("Cantidad habitantes") {
            steps {
               println cantidadHabitantes 
            }
        }
        stage("Población neta") {
            steps {
                script {
                    calcularPoblacionNeta(cantidadPoblacion)
                }
            }
        }
    }
}

def calcularPoblacionNeta (int cantidadPoblacion) {
    println cantidadPoblacion / 2
}
