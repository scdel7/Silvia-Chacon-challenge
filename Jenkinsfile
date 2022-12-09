pipeline {
    agent {
        label 'qa'
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
