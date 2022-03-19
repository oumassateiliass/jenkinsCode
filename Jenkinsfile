pipeline {
  agent any
     stages {
     stage("REMINDER_NOTIFICATIONS_PROD") {
  		steps {
  			script {
				final String url = 'https://betternight.com/service/v1/message/reminder/email?pwd=J3$gqpK9vwf4'
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}