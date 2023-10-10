pipeline {
    agent any
    stages {
       stage('git') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: 'projet_achat']], userRemoteConfigs: [[url: 'https://github.com/Maryam1818/projet_achat.git']]])
              
            }
        }
       stage('maven clean compile') {
            steps { 
               sh'mvn clean'
	       sh'mvn compile'
		}
        }
        }
       
    }

