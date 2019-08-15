    
pipeline {
  
  agent any
    
  tools {nodejs "Nodejs"}
    
  stages {
        
    stage('Code checkout') {
      steps {
        git 'https://github.com/vasurampalli/hello-world-node-package'
        sh 'node -v'
        sh 'npm -v'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    } 
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }
    stage('build') {
      steps {
         sh 'npm build'
      }
    }
    stage('Deploy') {
      steps {
         sh 'npm deploy'
      }
    }  
    stage('start') {
      steps {
         sh 'npm start'
      }
    }
  }
}
