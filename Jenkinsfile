pipeline{
	agent any
	tools {
  maven 'maven3'
        }

	stages{
	 stage('Git checkout'){
	   steps{
	  git credentialsId: 'gitHub',
	  url: 'https://github.com/Apurb1994/Apurb-Devops'
	}
 	}
 
  stage('mvn clean package'){
	   steps{
	 sh 'mvn clean package'
	}
 	}


  }
}
