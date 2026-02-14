pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/subhamsourabh5858-collab/sparkjava-war-example.git', branch: 'master'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
