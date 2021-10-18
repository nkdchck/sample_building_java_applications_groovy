@Library('jenkins-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
