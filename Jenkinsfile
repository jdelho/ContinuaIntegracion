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
            echo "El clima es lluvioso"
        break
        case 2: 
            echo "Martes"
            echo "Suma 150 + 350 = " + new Integer(150) + new Integer(350)
        break
        case 3: 
            echo "Miercoles"
            echo "Numero PI: " + Math.PI
        break
        case 4: 
            echo "Jueves"
            wrap([$class: 'BuildUser']) {
                echo "Usuario: $BUILD_USER"
            }
        break
        case 5: 
            echo "Viernes"
            echo "Version JAVA: "
            bat "java -version"
        break
        case 6: case 7: 
            echo "Fin de semana"
            echo "¡Descanso!"
        break
        default:
            echo "Error al obtener el dia: " + dia
        break
    }
}
