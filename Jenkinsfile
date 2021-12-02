pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo 'Hello'
            }
        }
        stage('Test') {
            steps {
                sh '/usr/bin/phpunit tests'
            }
        }
    }
    post {
        always {
            junit testResults: 'logs/unitreport.xml'
        }
    
    }
}
