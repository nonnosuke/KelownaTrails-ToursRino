pipeline {
    agent any

    stages {
        
	stage('Build') {
            steps {
                echo 'Nothing to do!' 
            }
        }

        stage('Test') {
            steps {
                echo This is testing.'
            }
        }

        stage('Staging') {
            steps {
                echo 'This is Staging.'
            }
        }

        stage('Production') {
	     steps {
                sh 'firebase use production'
                sh 'firebase deploy --only hosting'
            }
        }
    }
}
