pipeline {
    agent any
    stages {
       stage('git') { 
            steps { 
               checkout([$class: 'GitSCM', branches: [[name: 'master']], userRemoteConfigs: [[url: 'https://github.com/Maryam1818/projet_achat.git']]])
              
            }
        }
       stage('maven clean compile') {
            steps { 
               sh'mvn compile'
		}
        }
	      stage('maven sonarqube') {
            steps { 
                    sh 'mvn sonar:sonar -Dsonar.host.url=http://192.168.33.10:9000 -Dsonar.login=sonar'
                
		}
        }
        }
       
    }

