pipeline {    
  agent {        
    node{            
      label 'principal'        
    }   
  }    
  stages {        
    stage('Build') {             
      steps {
        bat 'cd AAA'
        bat 'mvn -B -DskipTests clean package'            
      }        
    }    
  }
}
