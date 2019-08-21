pipeline {
    agent any

    stages {
        stage('Build') {
	    steps {
                echo 'Building..'
		sh"docker build -t jenkins-master-slave Dockerfile"
		
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
