pipeline {
    agent any

    stages {
        stage('Build') {
	    steps {
                echo 'Building..'
		sh"fastlane init"
		
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
