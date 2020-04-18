pipeline {
	//agent any
	agent { docker { image 'node:13.8'}}
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
