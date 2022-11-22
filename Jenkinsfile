pipeline {
    agent any

    stages {
        stage("Top peliculas") {
            steps {
                println topPeliculas
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
    echo new Date().getTime()
}
