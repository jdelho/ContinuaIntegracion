pipeline {
    agent any 
    
    stages {
        stage("Comprobar fecha") {
            steps {
                script {
                    int dia = new Date().getDay()
                    switch(dia) {
                        case 1: {
                            echo "Lunes"
                            echo "El clima es lluvioso"
                        }
                        break
                    }
                }
            }
        }
    }
}
