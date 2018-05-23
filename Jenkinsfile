pipeline {
    agent any

    stages {
        stage('package') {
            steps {
                sh 'mvn clean package'
        steps {
         shell('''
            |cd target
            |curl -v -F r=test-release -F hasPom=false -F e=war -F g=dev.tech.ops -F a=project -F v=1.0 -F p=war -F file=@project.war -u admin:admin123 http://35.227.70.186:8081/repository/test-release/
              '''.stripMargin()
        )
    }
            }
        }
    }
}
