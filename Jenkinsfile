pipeline {
    agent any
    stages {
    	stage('creating war file'){
              steps {
                 sh '''
                      sudo yum install -y  maven
                      mvn clean install
                    '''
                    }
                  }
              }
    	}

