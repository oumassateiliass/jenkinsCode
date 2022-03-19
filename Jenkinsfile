pipeline {
  agent any
     stages {
     stage("SEND_EMAIL_NOTIFICATIONS_PROD") {
  		steps {
  			script {
				final String url = "https://betternight.com/service/v1/message/send/email?pwd=Mdg@ff5r2342"
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}