pipeline {
    agent any
    stages {
    	stage('creating war file'){
              steps {
                 sh '''
                      sudo yum install -y  maven
                    '''
                    }
                  }
        stage('clone repo'){
            steps {
                git url: 'https://github.com/AndriyKalashnykov/tomcat-root-war'
              }
    	}
        stage ('Build') {
               steps {
                   sh '''
                   cd tomcat-root-war
                   mvn clean install
                   '''
               }
               }
               }
               }

