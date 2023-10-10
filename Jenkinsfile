pipeline {
    agent any
    stages {
     
        stage('git') {
            steps {
                sh 'rmdir  /s /q projet_achat'
               sh 'git clone https://github.com/Maryam1818/projet_achat.git'
              
            }
        }
        stage('maven clean') {
            steps {
                sh 'mvn clean -f'
        	sh 'mvn -v'
			}
        }
       
        }
       
    }

