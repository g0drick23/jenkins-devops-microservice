//SCRIPTED
//DECLARATIVE

pipeline {
	agent any
	//agent { docker { image 'maven' } }
	//agent { 
	//	docker { image 'node:19.9' } 
	//}
	stages{
		stage("Build"){
				steps{
					//sh 'mvn --version'
					sh 'node --version'
					echo "Build"
				}			
			}
		stage("Test"){
				steps{
					echo "Test"
				}			
			}
		stage("Integration Test"){
				steps{				echo "Integration test"
				}			
			}				
	}
	post {
		always {
			echo "Im awesome. i run always"
		}
		success {
			echo "i run when you are successful"
		}
		failure{
			echo "I run when you fail"
		}

	}
}	
