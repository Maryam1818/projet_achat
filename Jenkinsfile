pipeline {
    agent any
    stages {
        stage('git') {
            steps {
               bat "rmdir  /s /q projet_achat"
               bat "git clone https://github.com/Maryam1818/projet_achat.git"
              
            }
        }
        stage('maven clean') {
            steps {
                bat "mvn clean -f projet_achat"
            }
        }
       
        }
       
    }

