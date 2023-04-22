//SCRIPTED
//DECLARATIVE

pipeline {
	//agent any
	agent { docker { image 'maven:3.6.3' } }
	stages{
		stage("Build"){
				steps{
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
//CHANGED



	}
}	
