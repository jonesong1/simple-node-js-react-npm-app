pipeline {
    agent any
    tools {nodejs "NodeJs"}
        
    stages {
        stage('Git') {
          steps {
            git 'https://github.com/jonesong1/simple-node-js-react-npm-app.git'
          }
        }

        stage('Build') {
          steps {
            sh 'npm install'
             sh '<<Build Command>>'
          }
        }  

        stage('Test') {
          steps {
            sh 'node test'
      }
    }
  }
}
