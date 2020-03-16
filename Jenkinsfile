pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh './mvnw clean compile' 
            }
        }
	stage('Test') {
            steps {
                sh './mvnw test' 
            }
        }
	stage('package') {
            steps {
                sh './mvnw package' 
            }
        }
	stage('Deploy') {
            steps {
                echo 'Deplotment stage ... Passed'
            }
        }
    }
}

