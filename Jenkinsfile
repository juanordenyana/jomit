pipeline {
    agent {
        node {
            label 'principal'
        }
    }
    environment {
        PATH = "$PATH/AAA"
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
