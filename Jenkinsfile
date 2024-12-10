pipeline {
    agent any
    tools{ jdk 'JDK19' }
    environment { JAVA_HOME = 'C:\\Program Files\\Java\\jdk-19' }
    stages {
       stage ('Compile Stage') {
        steps {
          withMaven(maven : 'MAVEN3.3.9windows') {
            bat 'mvn clean compile'
          }
        }
     stage ('Testing Stage') {
     steps {
     withMaven(maven : 'MAVEN3.3.9windows') {
bat 'mvn test'
} }}
stage ('Install Stage') {
steps {
withMaven(maven : 'MAVEN3.3.9windows') {
bat 'mvn install'
} } } }}
