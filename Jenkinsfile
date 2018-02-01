pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                //withMaven(maven : 'maven3.3.9') {
		     
		    bat 'set M2_HOME=C:\Devops software\apache-maven-3.5.2'
		    bat "set path =C:\Devops software\apache-maven-3.5.2"
		    bat 'mvn -version'
                    bat 'mvn clean compile'
            //   }

			  
			  // Added new comment
		    // added new line
			}
        }

        stage ('Testing Stage') {

            steps {
               // withMaven(maven : 'maven3.3.9') {
                    
		    bat  'mvn test'
               // }
            }
        }


        stage ('Deployment Stage') {
            steps {
              //  withMaven(maven : 'maven3.3.9') {
                    bat 'mvn install'
               // }
            }
        }
    }
}
