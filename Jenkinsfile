pipeline {
    agent any
    
    tools {
        jdk 'jdk17'
        maven 'maven3'
    }
    
    environment {
        IMAGE_TAG = "${BUILD_NUMBER}"
    }
    
    stages {
        
        stage('Git Checkout'){
           steps {
               echo ' git branch https://github.com/darekarankita0/jenkis-demo.git'
                
           }
        }
        
        stage('Compile using Maven'){
           steps {
               echo 'sh mvn compile'
                
           }
        }

        stage('Test using Maven'){
           steps {
               echo 'sh mvn test'
                
           }
        }

        
        stage('SonarQube Analysis'){
           steps {
               echo 'SonarQube Analysis'
                
           }
        }
        
        stage('Quality Gate'){
           steps {
               echo 'Quality Gate'
                
           }
        }
        
        stage('Build'){
           steps {
               echo 'sh mvn package'
                
           }
        }
        
        stage('Build & Tag Docker Image'){
           steps {
               echo 'Build & Tag Docker Image'
                
           }
        }
        
        stage('Push Docker Image'){
           steps {
               echo 'Push Docker Image'
                
           }
        }
        
        stage('Deploy to Kubernetes'){
           steps {
               echo 'Deploy to Kubernetes'
                
           }
        }

        stage('Verify the Deployment'){
           steps {
               echo 'Verify the Deployment'
                
           }
        }
}
}
