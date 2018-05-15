pipeline {
    agent any

    stages {
        stage('package') {
            steps {
                sh 'mvn package'
            }
             
        }
        stage('scp') {
            steps {
                sh 'scp target/project.war dinesh@35.227.70.186:/home/dinesh/'
            }
        }
         stage('') {
            steps {
                sh ''
            }
        }
    }
}
