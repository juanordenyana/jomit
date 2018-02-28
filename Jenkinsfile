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
                dir(pwd()+'/AAA')
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
