pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
	int build_tag_res = sh script: "docker build -t ${full_image_name} Dockerfile", returnStatus: true
        boolean build_tag = (build_tag_res == 0)

        if (!build_tag) {
            log.error 'There was an error tagging the image.'
            return
        }
	else{
log.error '$(build_tag_res)'
}

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
