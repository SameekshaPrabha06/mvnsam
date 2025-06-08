pipeline{
	agent any
	tools{
		maven 'Maven'
	}
	stages{
		stage('checkout'){
			steps{
				git branch:'master',url:'https://github.com/SameekshaPrabha06/mvnsam.git'
			}
		}
		stage('build'){
			steps{
				sh 'mvn clean package'
			}
		}
		stage('test'){
			steps{
				sh 'mvn test'
			}
		}
		stage('run'){
			steps{
				sh 'java -jar target/mvnsam-1.0-SNAPSHOT.jar'
			}
		}
	}
}
																							
