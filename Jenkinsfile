pipeline {
    agent {
        node {
            label 'principal'
        }
    }
    environment {
        PATH = "$pwd()/AAA"
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
