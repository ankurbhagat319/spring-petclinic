pipeline {
    agent {
            label 'master'
    }
    tools{
        maven 'maven3'
        jdk 'jdk8'
    }
    stages {
        stage('validate') {
            steps {
                sh 'mvn validate'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
         stage('package') {
            steps {
                sh 'mvn package'
            }
        }

    }
}
