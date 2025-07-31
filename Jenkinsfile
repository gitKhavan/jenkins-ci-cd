pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo 'Build'
			}
			post {
				always {
					echo 'I run at the end of Build stage'
				}
			}
		}
		stage('Test') {
			steps {
				echo 'Test'
			}
		}
		stage('Integration Test') {
			steps {
				echo 'Integration Test'
			}
		}
	}

	post {
		always {
			echo 'I always run'
		}
		success {
			echo 'I run when successful'
		}
		failure {
			echo 'I run when failed'
		}
	}
}