pipeline {
    agent any

    stages {
        stage('Checkout') {
            checkout scm
        }
        stage('Build') {
            sh 'python setup.py install'
        }
        stage('Test') {
            sh 'python -m unittest tests'
        }
    }
}
