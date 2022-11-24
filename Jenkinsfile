pipeline {
    agent any 
    
    stages {
        stage("Model Examen 1") {
            steps {
                script {
                    echo "Dia real:"
                    comprobarDia(new Date().getDay())
                    echo "Comprobar resto de dias:"
                    comprobarDia(1)
                    comprobarDia(2)
                    comprobarDia(3)
                    comprobarDia(4)
                    comprobarDia(5)
                    comprobarDia(6)
                    comprobarDia(7)
                    comprobarDia(8)
                }
            }
        }
    }
}

def comprobarDia(int dia) {
    switch(dia) {
        case 1: 
            echo "Lunes"
            int numero1 = 10
            int numero2 = 5
            println "Operaciones con numeros " + numero1 + " y " + numero2
            println "Suma = " + (numero1 + numero2)
            println "Resta = " + (numero1 - numero2)
            println "Multiplicacion = " + (numero1 * numero2)
            println "Division = " + (numero1 / numero2)
        break
        case 2: 
            echo "Martes"
            echo "Usuario: Jose Luis Del Hoyo Fernandez"
        break
        case 3: 
            echo "Miercoles"
            echo "¡Pipeline ejecutado!"
        break
        case 4: 
            echo "Jueves"
            echo "Clima: Lluvioso"
        break
        case 5: case 6: case 7:
            echo "Viernes, Sabado o Domingo"
            echo "No se han indicado acciones para estos dias"
        break
        default:
            echo "Error al obtener el dia: " + dia
        break
    }
}
