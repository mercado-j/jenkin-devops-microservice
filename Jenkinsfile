pipeline {
		// agent any
		agent {docker {image 'node:alpine:3.18'}}
		stages {
			stage('build') {
				steps {
					sh 'node --version'
					echo "Build"
				}
			}
			stage('Test') {
				steps {
					echo "Test"
				}
			}
			stage('Intergration') {
				steps {
					echo "Intergration Test"
				}
			}
		}
		post {
			always {
				echo 'Im awesome. I run always'
			}
			success {
				echo 'I run only when you are succesful'
			}
			failure {
				echo ' I run when you fail'
			}
		}
}
			
		
	
