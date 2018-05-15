pipeline {
    agent any
    environment {
            FILENAME = '${basename target/*.war}'
    VERSION = '${FILENAME:13:-4}'
    WAR = 'project-$VERSION.war'
      }
 
    stages {
        stage('package') {
            steps {
                sh 'mvn clean install package'
            }
        }
         
        stage('Example') {
 
               steps {             
    
                sh 'scp target/$WAR dinesh@35.227.70.186:/home/dinesh/'
              }          
        }

   }
}
