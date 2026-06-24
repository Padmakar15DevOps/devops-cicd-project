pipeline {
agent any


stages {

    stage('Build Docker Image') {
        steps {
            bat 'docker build -t devops-app .'
        }
    }

    stage('Remove Old Container') {
        steps {
            bat 'docker rm -f devops-container'
        }
    }

    stage('Run Container') {
        steps {
            bat 'docker run -d -p 80:80 --name devops-container devops-app'
        }
    }

}


}

