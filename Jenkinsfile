pipeline {
agent any

stages {

stage ('Complile stage'){
            steps { 
                  withMaven(maven : 'maven_3_5_0'){
                  sh 'mvn clean compile'
                        }
                   }
            }

stage('Testing Stage'){
                   steps {
                   withMaven(maven : 'maven_3_5_0'){
                   sh 'mvn test'
                   }
                 }
              }
              
stage('Deployment stage'){
                   steps {
                    withMaven(maven : 'maven_3_5_0'){
                   sh 'mvn deploy'
                   }
                }
             }
 }
 }
               


 
