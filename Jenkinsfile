pipeline {
	agent any
    stages {
		stage('Build') {
			steps {
				echo "Build"
				echo "$PATH"
				echo "$BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL -$env.BUILD_URL"
				echo "JOB_NAME -$env.JOB_NAME"
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
