pipeline {
    agent any

    stages {
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
    int hours = new Date().getHourOfDay()
    println hours
}
