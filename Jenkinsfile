pipeline{
	// agent any
	agent { docker { image 'maven:3.9.5-eclipse-temurin-11'} }
	stages {
		stage('Build'){
			steps{
				sh 'nvm --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}			
		}
		stage('Integration Build'){
			steps{
				echo "Integration Build"
			}
		}
	} 
	post {
		always {
			echo "I run always" 
		}
		success {
			echo "I run when you are success"
		}
		failure {
			echo "I run when you fail"
		}
	}
}