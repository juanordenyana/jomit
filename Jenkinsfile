pipeline {
    agent {
        node{
            label 'principal'
        }
    }
    stages {
        stage('Build') { 
            steps {
                cmd 'mvn -B -DskipTests clean package'
            }
        }
    }
}
