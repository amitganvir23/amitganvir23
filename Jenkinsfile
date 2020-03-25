node("master"){

        stage("Checkout"){
            ws("pipline-workspace") {
    			if (RERUN=="false") {
    			    cleanWs()
    			}
				git credentialsId: 'github', branch: 'master', url: "$PROJECT_REPO"
    		}
    	}

}

pipeline {
    agent any
    tools {
        maven 'maven-3.6.3'
        jdk 'java version 13.0.2'
    }
    
    stages {
        stage ("initialize") {
            steps {
                dir("lcd"){
                
                }
            }
        }
    }

}
