//First Test
//node {
//	stage('Build') {
//		echo "Build"
//	}
//	stage('Test') {
//		echo "Test"
//	}
//	stage('Integration Test') {
//		echo "Test"
//	}
//}
//SCRIPTED 2 test
//node {
//	echo "Build"
//	echo "Test"
//	echo "Integration Test"
//}
//declarative 
pipeline {
	//agent any
	//agent { docker {image 'maven:3.6.3'}}
	agent { docker {image 'node:14.2'}}
	stages {
		stage('Build') {
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
		stage('IntegrationTest') {
			steps {
				echo "Integraton Test"
			}
		}
	} 
	post {
		always  {
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}