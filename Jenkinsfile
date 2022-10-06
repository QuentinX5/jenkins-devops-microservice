//SCRIPTED
/*
node {
	echo "Build"
	echo "Test"
	echo "Test"
}
*/

//DECLARATIVE
pipeline {
	//agent { docker { image 'maven:3.6.3' } }
	//agent any
	agent { docker { image 'node:latest' } }
	stages {
		stage('Build'){
			steps {
				sh "node --version"
				echo "Build"
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps {
				echo "Test"
			}
		}
	}
	
	post {
		always {
			echo "I am awesome. I run always."
		}
		success {
			echo "I run when you are successful."
		}
		failure {
			echo "I run when you fail."
		}
	}
}
