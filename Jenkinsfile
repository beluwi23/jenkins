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
//decclarative 
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
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
}