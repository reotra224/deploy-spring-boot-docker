pipeline {
    agent { 
    	docker { 
    		image 'maven:3.3.3' 
    		image 'node:7-alpine'
    	}
    }
    
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'java -version'
                sh '''
                	echo "Multiline shell steps works too"
                    ls -la
                '''
            }
        }
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}