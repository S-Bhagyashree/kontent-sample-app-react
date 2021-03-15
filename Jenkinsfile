pipeline {

	agent any

	stages {

		stage('install dependencies') {
			steps {
				sh 'npm install'
			}
		}
			
		stage('Build') {
			steps {
				sh 'npm run build'
			}
		}

		stage('Test') {
			steps {
				sh 'npm test'
			}
		}

		stage('Deploy') {
			steps {
				sh 'npm start &'
			}
		}
	
  }
}
