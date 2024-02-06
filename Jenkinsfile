pipeline {
		agent any
		// agent {docker {image 'node:13.8'}}
		stages {
			stage('build') {
				steps {
					// sh 'node --version'
					echo "Build"
					echo "PATH - $PATH"
					echo "BUILD_NUMBER - $env.BUILD_NUMBER"
					echo "BUILD_ID - $env.BUILD_ID"
					echo "JOB_NAME - $env.JOB_NAME"
					echo "BUILD_TAG - $env.BUILD_TAG"
					echo "BUILD_URL - $env.BUILD_URL"
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
			
		
	
