@Library('jenkins-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                checkout scm
                sh './gradlew build'
            }
        }
        stage('Shared Library Test') {
            steps {
                welcome("Rick Sanchez")
                script {
                    calculator.add(3, 3)
                    calculator.mul(3, 5)
                } 
            } 
        }
    }
}
