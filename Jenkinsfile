pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
          }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/Kashi779/webapp-project.git', branch: 'main'
            }
        }
        stage('Maven Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        
    }
}
