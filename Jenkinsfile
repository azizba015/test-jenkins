pipeline {
    agent any
    stages {
	stage('Checkout code') {
            steps {
               checkout scm
                  }
        }
        stage('Install dependencies application') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test application') {
            steps {
                sh 'npm test'
            }
        }
        stage('Launch application') { 
            steps {
                sh 'npm start &' 
            }
        }
    }
}
