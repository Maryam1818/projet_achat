pipeline {
    agent any
    stages {
       stage('git') { 
            steps { 
               checkout([$class: 'GitSCM', branches: [[name: 'master']], userRemoteConfigs: [[url: 'https://github.com/Maryam1818/projet_achat.git']]])
            }
        }
	    
	stage('compiling') {
            steps { 
		    sh 'mvn clean' 
		}
        }
	stage('SONARQUBE') {
            steps {
                sh'mvn sonar:sonar -Dsonar.host.url=http://192.168.33.10:9000 -Dsonar.login=sonar'
            }
        }

	}
    }

