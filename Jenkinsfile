pipeline {
    agent {
        node {
            label 'principal'
        }
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
