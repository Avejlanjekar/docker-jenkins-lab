pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                checkout scm
            }
        }

        stage ('Docker build'){
            steps{
                sh "docker build -t docker-jenkins-lab ."
            }
        }
    }
}