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
                sh 'scp target/project.war dinesh@35.227.70.186:/opt/'
            }
        }
         stage('') {
            steps {
                sh ''
            }
        }
    }
}
