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

        stage ('Docker Tag'){
            steps{
                sh "docker tag docker-jenkins-lab avejlanjekar45/jenkins-docker-lab"
            }
        }
    }
}