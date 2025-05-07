pipeline {
    agent {label: instance-java}
    stages {
       stage('running playbook') {
         steps {
             sh '''
               ansible-playbook -i inventory.ini playbook.yml
                '''
             }
          }
    	stage('creating war file'){
              steps {
                 sh '''
                      mvn clean install
                    '''
                    }
                  }
             stage(' changing the root directory'){
               steps {
                  sh '''
                      cp ./target/ROOT.war  opt/tomcat/webapps/ROOT.war
                     '''
                     }
                 }
              }
    	}

