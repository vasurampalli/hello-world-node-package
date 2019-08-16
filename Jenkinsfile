    
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
        echo 'Installing'
      }
    } 
    stage('Test') {
      steps {
         sh 'npm test'
         echo 'Testing'
      }
    }
    stage('build') {
      steps {
         sh 'npm build'
         echo 'Building'
      }
    }
    stage('deploy') {
      steps {
         sh 'npm config ls'
         echo 'deploying'
      }
    }
    stage('start') {
      steps {
         sh 'npm start'
         echo 'starting'
      }
    }
  }
}
