#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:3.9.1-eclipse-temurin-17'
                label 'docker-maven'
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
  }
}
