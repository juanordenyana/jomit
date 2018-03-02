pipeline {
    agent {
        node {
            label 'principal'
        }
    }
    stages {
        stage('Build') {
            steps {
                dir(pwd()+'\\AAA'){
                    bat 'mvn -B -DskipTests clean package'
                }
            }
        }
        stage('Deploy'){
            steps{
                dir(pwd()+'\\AAA'){
                    bat 'mvn deploy -DrepositoryId=jomit -Durl=http://localshots:9091'
                }
            }
       }
    }
}
