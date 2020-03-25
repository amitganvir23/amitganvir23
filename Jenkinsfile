node("master"){

        stage("Checkout"){
            ws("pipline-workspace") {
    			cleanWs()
				git credentialsId: 'github', branch: 'master', url: "https://github.com/amitganvir23/hello_gradle.git"
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
