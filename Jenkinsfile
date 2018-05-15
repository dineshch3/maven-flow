pipeline {
    agent any
    
    stages {
        stage('package') {
            steps {
                sh 'mvn clean install package'
            }
             
        }    
        stage('Example') {
             environment { 
        FILENAME = '${basename target/*.war}'
    VERSION = '${FILENAME:13:-4}'
    WAR = 'modelmanager-$VERSION.war'

              steps {
                sh 'scp target/$war dinesh@35.227.70.186:/home/dinesh/'
              }          
  }
        }

}
}
