pipeline {
    agent any
    stages {
        stage('Maven version') {
            steps {
                        bat 'mvn -v'
            }
        }
        stage('Running Test') {
            steps {
                        git credentialsId: 'f32cc775-1ad8-42a0-b368-fad115b8e44a', url: 'https://github.com/hemalathacsg/SBforDecScripted.git'
            }
        }
        stage('Build') {
            steps {
                   bat 'mvn  clean test'
            }
        }
    }
}