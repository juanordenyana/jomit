pipeline {
    agent {
        node {
            label 'principal'
        }
    }
    stages {
        stage('Build') {
            steps {
                bat 'cd AAA mvn -B -DskipTests clean package'
            }
        }
    }
}
