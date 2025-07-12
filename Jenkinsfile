pipeline{
 tools{
        jdk 'JAVA_HOME_LINUX'
        maven 'M2_HOME_LINUX'
    }
     agent {label 'linuxos'}  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git 'https://github.com/ashisnishanka/jenkins-maven-repo.git'
	   }
	                  }
	
	   stage("compile"){
	    steps{
		 sh 'mvn compile'
		}
		}
		stage("test"){
	    steps{
		 sh 'mvn test'
		}
		}
		stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
		stage("install"){
	    steps{
		 sh 'mvn install'
		}
		}
	  }
	}
