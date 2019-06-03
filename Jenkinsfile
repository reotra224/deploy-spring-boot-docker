pipeline {
    agent { 
    	docker {
	        image 'node:7-alpine'	        
	    }
    }
    
    stages {
        stage('build and Test') {
            steps {
                sh '''
                	echo "Multiline shell steps works too"
                    ls -la
                '''
                sh 'node --version'
            }
        }
//        stage('Test') {
//            steps {
//                sh 'node --version'
//            }
//        }
    }
}