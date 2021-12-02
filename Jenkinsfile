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
                sh '/usr/bin/phpunit --log-junit logs/unitreport.xml -c tests/phpunit.xml tests'
            }
        }
    }
    post {
        always {
            junit testResults: 'logs/unitreport.xml'
        }
    
    }
}
