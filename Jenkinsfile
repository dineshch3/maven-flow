pipeline {
    agent any

    stages {
        stage('package') {
            steps {
                sh 'mvn clean install package'
            }
             
        }
        environment {
    FILENAME="$(basename target/*.war)"
    VERSION="${FILENAME:13:-4}"
    WAR="modelmanager-$VERSION.war"
  }
        stage('scp') {
            steps {
                sh 'scp target/$war dinesh@35.227.70.186:/home/dinesh/'
            }
        }
         stage('') {
            steps {
                sh ''
            }
        }
    }
}
