pipeline {
    agent any
    stages {
        stage('Build Dockerfile') {
                // script {
			    //     dockerImage = docker.build("flask-example")
		        // }
            agent {
                docker {
                    image 'flask-example'
                    reuseNode true
                }
            }
            steps {
                docker ps
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
