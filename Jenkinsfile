pipeline {
    agent any
    stages {
    	stage('creating war file'){
              steps {
                 sh '''
                      yum install mvn
                      mvn clean install
                    '''
                    }
                  }
              }
    	}

