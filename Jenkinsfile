pipeline {
     agent any
//      tools {
//         gradle "gradle"
//     }
     stages {
         stage('Clean Workspace') {
             steps {
                  deleteDir()                  
             }
         }
         stage('Clone Project') {
             steps {                  
                  checkout scm                  
             }
         }
         stage('Build') {
             steps {    
                  sh '/usr/bin/gradle clean build'
             }              
         }
     }
 }
