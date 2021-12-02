pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo '1234'
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
