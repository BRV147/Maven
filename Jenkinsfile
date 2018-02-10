pipeline {
    agent {
        docker 'maven' 
    }
    tools{
        maven 'maffin'
    }
    stages {
        stage('Start') {
            steps {
                git 'https://github.com/BRV147/Maven.git'
            }
        }
        stage('Function') {
            steps{
                sh "mvn package"
            }
        }
    }

}
