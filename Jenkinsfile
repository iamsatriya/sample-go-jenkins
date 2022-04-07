pipeline{
    agent any
    stages{
        stage("Build & Test"){
            agent {
                docker {
                    image 'golang:alpine'
                }
            }
            steps{
                echo "========Build and Test========"
                sh 'go version'
            }
        }
    }
}