pipeline {
    agent { 
    	docker { 
    		image 'maven:3.3.3' 
    	}
    }
    
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'java -version'
                sh '''
                	echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}