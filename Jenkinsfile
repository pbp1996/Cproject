pipeline {
    agent any
    stages {
        stage('BUILD') {
            parallel {
            stage('BUILD1') {
           steps {
             echo " This is build steps "
             sh " sleep 5 "
           }
        }
            stage('BUILD2') {
               steps {
                 echo " This is build steps "
                 sh " sleep 5 "
           }
        } 
     }
    }
        stage('DEPLOY') {
            agent { label 'agent1' }
           steps {
             echo " This is DEPLOY steps "
             sh " sleep 5 "
           }
        }
        stage('TEST') {
           steps {
             echo " This is Test steps "
             sh " sleep 5 "
           }
        } 
    }
}  
            
                
               
            
