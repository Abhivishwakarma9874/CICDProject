@Library("Shared") _
pipeline {
    agent { label 'for_agent' }

    stages {

        stage('Code') {
            steps {
                script {
                    cloneRepo('https://github.com/Abhivishwakarma9874/CICDProject.git', 'main')
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    buildImage('cicdproject:latest')
                }
            }
        }

        stage('Push to DockerHub') {
            steps {
                script {
                    pushToDockerHub('cicdproject:latest', 'dockerhubcredential')
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    sh 'docker compose up -d'
                }
            }
        }
    }
}
