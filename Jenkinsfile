pipeline {
    agent any

    stages {
        stage('git cloning') {
            steps {
                git 'https://github.com/vigneshtraining/jenkinstraining.git'
            }
        }
        stage('am compiling') {
            steps {
                echo "Am compiling here"
                sh '/usr/bin/mvn compile'
            }
        }
        stage('am testing') {
            steps {
                sh '/usr/bin/mvn test'
            }
        }
        stage('am packaging') {
            steps {
                sh '/usr/bin/mvn package'
            }
        }
         
    }
}
