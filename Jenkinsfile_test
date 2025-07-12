pipeline{
 tools{
        jdk 'JAVA_HOME_MASTER'
        maven 'M2_HOME'
    }
     agent any
	  
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
		stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
	  }
	}
