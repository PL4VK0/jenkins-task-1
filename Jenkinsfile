pipeline {
    agents any
    environment {
        APP_PORT = '9090'
      }
    stages {
          stage ('Build') {
              steps {
                  sh 'mvn -B package -Dskiptests'
                }
            }
          stage ('Test') {
              steps {
                  sh 'mvn -B test'
                }
            }
      }
  }
