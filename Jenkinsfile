pipeline {
    agent {
        node {
            label 'principal'
        }
    }
    stages {
        stage('Build') {
            steps {
                dir(pwd()+'\AAA'){
                    bat 'mvn -B -DskipTests clean package'
                }
            }
        }
    }
}
