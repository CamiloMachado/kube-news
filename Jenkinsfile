pipeline {
    agent any

    stages {

        stages ('Build Docker Image') {
            step {
                script {
                    dockerapp = docker.build("camilomachado/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }


}