pipeline {
    agent any
    stages {
        stage('Build Dockerfile') {
            steps {
                script {
			dockerImage = docker.build("flask-example")
		}
            }
        }
        stage('Test') {
            steps {
                echo "test"
            }
        }
        stage('Deploy') {
            steps {
                echo "deploy"
            }
        }
    }
}
