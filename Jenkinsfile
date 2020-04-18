pipeline {
	//agent any
	agent { docker { image 'maven:3.6.3'}}
    stages {
		stage('Build'){
			steps {
				sudo sh "mvn --version"
				echo "Build"
			}
		}
				stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Intergaration Test'){
			steps {
				echo "Intergaration Test"
			}
		}

	} 
	post {
		always {
		 echo 'Im Awesome. I run alwyas'
		}
	  success {
		echo 'I run on sucess'
	  	}
	  failure {
		echo 'I run whn you fail'
	  	}

    }	
 
}
