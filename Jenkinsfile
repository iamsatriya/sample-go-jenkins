pipeline{
    agent any
    environment {
        module = "sample-go-jenkins"
        branch = "master"
        scmUrl =  "https://github.com/iamsatriya/sample-go-jenkins.git"
    }
    stages {
        stage("Git Clone") {
            steps {
                git branch: "${branch}", url: "${scmUrl}"
            }
        }
        stage("Go Dockerize") {
            steps {
                sh "docker build -t ${module}"
            }
        }
        stage("Deploy") {
            steps {
                sh "Deploy success"
            }
        }
    }
}