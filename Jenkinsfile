pipeline {
    agent any

    stages {
        stage('Build') {
	    steps {
                echo 'Building..'
		sh"docker build -t ankursingh081/jenkins-master-slave ."
		
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
