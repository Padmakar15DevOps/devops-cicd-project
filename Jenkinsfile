pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Padmakar15DevOps/devops-cicd-project.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build Successful'
            }
        }
    }
}
