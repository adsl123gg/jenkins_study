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
}
