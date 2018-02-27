pipeline {
    agent {
        node{
            label 'principal'
        }
    }
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
