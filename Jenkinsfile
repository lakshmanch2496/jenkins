pipeline {
    
	agent any
/*	
	tools {
        maven "maven3"
    }
*/	
    stages{
        
        stage(''clone repo''){
            steps { 
		    withCredentials(usernamePassword(credentialsId :jenkins-user-github ,passwordVariable: 'GIT_PASSWORD', usernameVariable: 'GIT_USERNAME' )){
              // Get some code from a GitHub repository
              bat("""
              git config --global credential.username {GIT_USERNAME}
              git config --global credential.helper "!echo password={GIT_PASSWORD}; echo"
              git clone https://github.com/aakashsehgal/FMU.git

              echo "pulled the code"
              """)

          }


         }

         }
      }

}
		    
                
