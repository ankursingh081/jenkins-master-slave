pipeline {
    agent any

    stages {
        stage('Build') {
	    steps {
                echo 'Building..'
		sh"/usr/bin/docker build -t ankursingh081/jenkins-master-slave Dockerfile"
		
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
