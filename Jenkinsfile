pipeline {
    agent any

    stages {
        stage('npm') {
            steps {
                sh 'npm install'
            }
             
        }
        stage('bower') {
            steps {
                sh 'bower install'
            }
        }
         stage('npm run prod') {
            steps {
                sh 'npm run prod'
            }
        }
    }
}
