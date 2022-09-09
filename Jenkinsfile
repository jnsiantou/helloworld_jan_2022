pipeline {
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages {
        stages {'Build') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
        }
            
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stages('Deploy') {
            steps {
                echo 'Deploy Step'
                sleep 10
            }
        }
        stage('Docker') {
            steps {
                echo 'Image step'
            }
              
        }
    }
}
      
    
