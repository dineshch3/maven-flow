
def giturl = "https://github.com/dineshch3/maven-flow.git"
def gibranch = "master"

pipeline {
    agent any

    stages {
        stage('package') {
            steps {
                script{
                    
                    git url: "${giturl}", git branch: "${gitbranch}" 
                  
                def mvnHome = tool 'M3'
                    
                sh 'mvn clean package'
                }
            }
        }
    }
}
