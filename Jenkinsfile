pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn package'
            }
             
        }
        stage('Transfer files') {
            steps {
                sh 'scp target/project.war dinesh@35.185.9.234:/home/dinesh/'
            }
        }
         stage('deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}
