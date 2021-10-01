//scripted
// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// }
// node {
// 	echo "Build"
// 	echo "Test"
// 	echo "Integration Test"
// }

//declarative
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
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}

	post {
		always {
			echo "I'm awesome. I run always."
		}
		success {
			echo "I run when I am successful."
		}
		failure {
			echo "I run when I fail."
		}
	}
	
}
