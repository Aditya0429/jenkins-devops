pipeline {
	agent any
    stages {
		stage('Build'){
			steps {
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
	  sucess {
		echo ' I run on sucess'
	  	}
	  failure {
		echo 'I run whn you fail'
	  	}

    }	
 
}
