pipeline {
    agent any
// testing the jenkins ***************
    stages {
        stage ('Compile Stage') {

            steps {
                //withMaven(maven : 'maven3.3.9') {
		     
		    bat 'set M2_HOME=C:/learning/software-dump/maven/apache-maven-3.3.9-bin/apache-maven-3.3.9'
		    bat "set path =C:/learning/software-dump/maven/apache-maven-3.3.9-bin/apache-maven-3.3.9/bin:%path%"
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
#12
