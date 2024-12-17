pipeline {
    agent any

    stages {
        stage('permission') {
            steps {
		sh 'clean'
                sh 'chmod 777 script2.sh'
		sh 'chmod 777 Script1.sh'
		sh 'echo "permission granted" '
            }
	}
	stage('execution') {
            steps {
                sh './script2.sh'
		sh './Script1.sh'
		sh 'echo "execution succesfull" '
            }
        }
	stage('Display') {
            steps {
                sh 'cat script2.sh'
		sh 'cat Script1.sh'
            }
	}
    }
}

