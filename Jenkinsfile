def nombre = "Jose Luis"
def numero1 = 1
def numero2 = 2
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage("Uso de variable universal") {
            steps {
               println nombre 
            }
        }
        stage("Mostrar fecha") {
            steps {
                script {
                    def dia = new Date()
                    println dia
                }
            }
        }
        stage("Calculadora") {
            steps {
                println numero1
                println numero2
                println numero1 + numero2
            }
        }
        stage("Condicionales") {
            steps {
                script {
                    if (numero1 == 1) {
                        echo "Numero válido"
                    } else {
                        echo "Numero no válido"
                    }
                }
            }
        }
        stage("Funcion") {
            steps {
                script {
                   mostrarVersionMaven("Versión maven")
                }
            }
        }
    }
}

def mostrarVersionMaven (String a) {
    echo a
    bat "mvn -v"
}
