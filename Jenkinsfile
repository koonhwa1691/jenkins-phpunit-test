pipeline {
	agent any {
		docker {
			image 'composer:latest'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'composer install'
			}
		}
		stage('Test') {
			steps {
                sh 'https://github.com/koonhwa1691/jenkins-phpunit-test/GumballMachine.php'
            }
		}
	}
}
