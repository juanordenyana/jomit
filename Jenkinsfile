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
                echo(pwd())
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
