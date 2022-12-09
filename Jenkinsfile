pipeline {
    agent {
        label 'qa-nodo'
    }

    stages {


        stage('Unit test') {
            steps {
                sh 'mvn test'
            }
            post {
                always {
                   junit 'target/surefire-reports/*.xml'
                }
            }
        }

       }
        }
