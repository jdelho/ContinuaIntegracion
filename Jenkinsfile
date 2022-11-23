pipeline {
    agent any 
    
    stages {
        stage("Comprobar fecha") {
            steps {
                script {
                    int dia = new Date().getDay()
                    switch(dia) {
                        case 1: 
                            echo "Lunes"
                            echo "El clima es lluvioso"
                        break
                        case 2: 
                            echo "Martes"
                            echo "El clima es lluvioso"
                        break
                        case 3: 
                            echo "Miercoles"
                            echo "El clima es lluvioso"
                        break
                        case 4: 
                            echo "Jueves"
                            echo "El clima es lluvioso"
                        break
                        case 5: 
                            echo "Viernes"
                            echo "El clima es lluvioso"
                        break
                        case 6: case 7: 
                            echo "Fin de semana"
                            echo "¡Descanso!"
                        break
                    }
                }
            }
        }
    }
}
