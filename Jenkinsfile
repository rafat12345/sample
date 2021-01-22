pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
         
            stage ('Copy .war file to tomcat') {
             steps {
                 sh '''
                       cp target/*.war $WORKSPACE
        
                    '''
             }
         }
    }
}
