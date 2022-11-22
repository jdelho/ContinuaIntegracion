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
    echo new Date().getTime()
}
