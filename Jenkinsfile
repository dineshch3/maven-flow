pipeline {
    agent any

    stages {
        stage('package') {
            steps {
                sh 'mvn clean install package'
            }
             
        }
        stage('scp') {
            steps {
                sh 'scp /var/lib/jenkins/workspace/jenkinsfile01/target/project.war nexus@35.227.70.186:/home/dinesh/'
            }
        }
         stage('') {
            steps {
                sh ''
            }
        }
    }
}
