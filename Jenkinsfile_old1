pipeline {
  tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
	
  agent any
  stages {
    stage('git clone')
	{
	 steps
	 {
	   git 'https://github.com/ashisnishanka/jenkins-maven-repo.git'
	 }
	
	}
	
	stage('compile')
	{
	 steps
	 {
	   sh 'mvn compile'
	 }
	
	}
	
	stage('package')
	{
	 steps
	 {
	   sh 'mvn package'
	 }
	
	}
	stage('install')
	{
	 steps
	 {
	   sh 'mvn install'
	 }
	
	}
  
  
  }
  
  
}
