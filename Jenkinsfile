pipeline {
    agent any
    stages {
	    
      stage('maven clean') {
            steps {
                sh 'mvn clean -f projet_achat'
        	sh 'mvn -v'
		}
        }
       
        stage('git') {
            steps {
                sh 'rmdir  /s /q projet_achat'
               sh 'git clone https://github.com/Maryam1818/projet_achat.git'
              
            }
        }
      
        }
       
    }

