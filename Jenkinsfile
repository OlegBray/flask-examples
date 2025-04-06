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
                sh 'docker ps'
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
