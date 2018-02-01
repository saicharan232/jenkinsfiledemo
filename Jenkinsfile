pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                //withMaven(maven : 'maven3.3.9') {
		     bat 'mvn -version'
		    bat 'set M2_HOME=C:\learning\software-dump\maven\apache-maven-3.3.9-bin\apache-maven-3.3.9'
		    bat "set path =%M2_HOME\bin%:%path%"
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
