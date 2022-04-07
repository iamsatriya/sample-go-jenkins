pipeline{
    agent {
        dockerfile true
    }
    stages{
        stage("Build & Test"){
            steps{
                echo "========Build and Test========"
                sh 'go version'
            }
        }
    }
}