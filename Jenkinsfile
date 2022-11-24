pipeline {
    agent any 
    
    stages {
        stage("Model Examen 1") {
            steps {
                script {
                    echo "Dia real:"
                    comprobarDia(new Date().getDay())
                    echo "Otras comprobaciones:"
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
            println "Suma: 10 + 5 = " + (int)10 + (int)5
            println "Resta: 10 - 5 = " + (int)10 - (int)5
            println "Multiplicacion: 5 * 10 = " + (int)5 * (int)10
            println "Division: 10 / 2 = " + (int)10 / (int)2
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
            echo "¡Descanso!"
        break
        default:
            echo "Error al obtener el dia: " + dia
        break
    }
}
