pipeline {
		// agent any
		agent {docker {image 'maven:3.6.3'}}
		stages {
			stage('build') {
				steps {
					echo 'mvn--version'
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
			
		
	
