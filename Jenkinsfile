pipeline {
    agent any 
    stages {
       stage('running playbook'){
         steps {
             sh '''
               ansible-playbook -i inventory.ini
                '''
             }
          }
