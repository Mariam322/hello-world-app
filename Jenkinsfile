pipeline {
    agent any
    tools{ jdk 'jdk8’ }
    environment { JAVA_HOME = 'C:\Program Files\Java\jdk-19' }
    stages {
       stage ('Compile Stage') {
        steps {
          withMaven(maven : 'apache-maven-3.9.9') {
            bat 'mvn clean compile'
          }
        }
     stage ('Testing Stage') {
     steps {
     withMaven(maven : 'apache-maven-3.6.1') {
bat 'mvn test'
} }}
stage ('Install Stage') {
steps {
withMaven(maven : 'apache-maven-3.6.1') {
bat 'mvn install'
} } } }}
