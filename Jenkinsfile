pipeline {
    agent any
    parameters {
        string(name:'APELLIDO')
        text(name:'BIOGRAFIA', description:'Ingrese su Biografia')
        booleanParam(name:'BOOLEAN')
    }
    environment {
        INSTAGRAM="Soy fking pipillas"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Fuck'){
            steps {
                echo "${INSTAGRAM}"
            }
        }
        stage('Print'){
            steps {
                echo "${env.BUILD_NUMBER}"
                echo "${BUILD_NUMBER}"
                echo "$BUILD_NUMBER"
            }
        }
        stage('Imprimir parametros'){
            steps {
                echo "${params.APELLIDO}"
            }
        }
        stage('Cambio variable'){
            steps {
                script  {
                    INSTAGRAM="Soy fking FLACO"
                    echo "${INSTAGRAM}"
                    
                }
                
            }
        }
    }
}