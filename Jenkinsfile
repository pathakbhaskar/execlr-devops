pipeline {
	agent any

	stages {
		stage('Fetching code from Git') {
			steps {
				git branch: 'main', url: 'https://github.com/pathakbhaskar/execlr-devops.git'
			}
		}

		stage('Installing Apache') {
			steps {
				sh 'sudo apt install apache2 -y'
			}
		}

		stage('Deploying website') {
			steps {
				sh 'sudo cp -R * /var/www/html/'
			}
		}

	}
}
