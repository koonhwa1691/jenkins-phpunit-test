pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo 'hello world'
            }
        }
        stage('Test') {
            steps {
                sh '/usr/bin/phpunit tests'
            }
        }
    }
}
