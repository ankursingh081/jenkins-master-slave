pipeline {
    agent any

    stages {
        stage('Build') {
	    steps {
                echo 'Building..'
		sh"docker build -t ankursingh081/jenkins-master-slave ."
#                boolean build_tag = (build_tag_res == 0)
#                if (!build_tag) {
#                        log.error 'There was an error tagging the image.'
#                        return
#                }
#                else{
#                        log.error '$(build_tag_res)'
#                }
		
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
