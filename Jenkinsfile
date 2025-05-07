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
                   mvn clean install
                   '''
               }
               }
        stage('running playbook'){
            steps {
                sh '''
                ansible-playbook -i /var/lib/jenkins/inventory.ini /var/lib/jenkins/playbook.yml
                '''
               }
               }
               }
               }

