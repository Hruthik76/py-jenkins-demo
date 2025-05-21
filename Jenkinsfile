pipeline {
    agent any

    environment {
        IMAGE = 'hruthik76/py-jenkins-demo:latest'
    }

    stages {
        stage('Pull Docker Image') {
            steps {
                echo "Pulling image: $IMAGE"
                sh '''
                    # Using Bash to pull the Docker image
                    docker pull $IMAGE
                '''
            }
        }

        stage('Run Docker Container') {
            steps {
                echo "Running container from image: $IMAGE"
                sh '''
                    # Using Bash to run the Docker container
                    docker run --rm $IMAGE
                '''
            }
        }
    }
}
