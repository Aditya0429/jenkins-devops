pipeline {
	//agent any
	//agent { docker { image 'node:13.8'}}
    stages {
		stage('Build'){
			steps {
				//sh "node --version"
				echo "Build"
				echo "$PATH"
				echo "$BUILD_NUMBER -$env,BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL -$env.BUILD_URL"
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
