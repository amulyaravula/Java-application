pipeline {
    agent any
    stages {
    	stage('creating war file'){
              steps {
                 sh '''
                      sudo yum install mvn
                      mvn clean install
                    '''
                    }
                  }
              }
    	}

