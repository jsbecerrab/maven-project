pipeline {
    agent any
    stages{
        stage('build'){
            steps{
                sh 'mvn clean package'
                sh "docker build . -tag tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }

       
}
