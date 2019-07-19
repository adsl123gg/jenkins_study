pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "print python version"'
		sh '''
			python --version
			pwd
		'''
            }
        }
    }
	
    post {
    success {
        mail to: 'adsl123gg2008@gmail.com',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "Something is wrong with ${env.BUILD_URL}"
    }
}
	
}
