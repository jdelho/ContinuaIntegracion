def topPeliculas = "Sinister, 1408, Veronica, Passengers, Independence Day"
def comidaFavorita = "Tortilla de patata con cebolla"
def signo = "Tauro"
def puesto = "Analista programador"

pipeline {
    agent any

    stages {
        stage("Top peliculas") {
            steps {
                println topPeliculas
            }
        }
        stage("Comida favorita") {
            steps {
               println comidaFavorita 
            }
        }
        stage("Signo zodiacal") {
            steps {
               println signo 
            }
        }
        stage("Puesto actual") {
            steps {
               println puesto 
            }
        }
        stage("Salario bruto > 1000") {
            steps {
                script {
                    calcularSalarioNeto(1100)
                }
            }
        }
        stage("Salario bruto < 1000") {
            steps {
                script {
                    calcularSalarioNeto(900)
                }
            }
        }
    }
}

def calcularSalarioNeto (int salarioBruto) {
    if (salarioBruto > 1000) {
        println salarioBruto * 0.80
    } else {
        println salarioBruto
    }
}
